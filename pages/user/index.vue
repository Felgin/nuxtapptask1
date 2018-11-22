<template>
	<article>
		<h1>User's List</h1>
		<section>
			<User 
			v-for="user in users"
			:key="user.id"
			:id="user.id"
			:name="user.name"
			:email="user.email"
			:phone="user.phone"
			:website="user.website"
			:companyname="user.company.name" 
			:companycatchPhrase="user.company.catchPhrase"
			:companybs="user.company.bs"
			/>
		</section>
	</article>
</template>

<script>
import axios from 'axios'
import User from '@/components/User' 

export default {
	components: {
		User
	},
	title: '',
	async asyncData () {
		const {data} = await axios.get('https://jsonplaceholder.typicode.com/users')
		return {users:data}
	}
}
</script>


<style scoped>
h1{
	margin-top: 20px;
	margin-bottom: 10px;
	text-align: center;
	text-transform: uppercase;
	font-family: sans-serif;
}
section{
	position: relative;
	display: flex;
	flex-flow: row wrap;
	justify-content: center;
	align-content: center;
	margin-bottom: 20px;
}
</style>
 