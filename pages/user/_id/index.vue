<template>
	<article>
		<div class="container">
            <h1>User Details</h1>
             <div class="usercontainer">
				<div>
					<ul>
						<li><b>Name:</b> {{ name }}</li>
						<li><b>Email:</b> {{ email }}</li>
                        <li><b>Username:</b> {{ username }}</li><br>
						<li><u><b>Address</b></u> <br><b>Street:</b> {{ address.street }}<br> <b>Suite:</b> {{address.suite}}<br><b>City:</b> {{address.city}}<br><b>Zipcode:</b> {{address.zipcode}}</li>
						<li><b>Phone:</b> {{ phone }}</li><br>
                        <li><u><b>Company and Details</b></u></li>
						<li><b>Website:</b> {{ website }}</li>
						<li><b>Company:</b> {{ company.name }}<br><b>CatchPhrase:</b> {{ company.catchPhrase }}<br><b>Bs:</b> {{ company.bs }}<br></li> 
                        <br>
                        <li> <nuxt-link to="/user">Back</nuxt-link></li>
					</ul>
				</div>          
             </div>
             </div>
	</article>
</template>

 <script>
 import axios from 'axios'

 export default {
   validate ({ params }) {
     return !isNaN(+params.id)
   },
   async asyncData({params, error}){
     const {data} = await axios.get(`https://jsonplaceholder.typicode.com/users/${+params.id}`)
     return data
   }
 }

 </script>


<style scoped>
article{
    margin-top: 20px;
	display: flex;
	justify-content: center;
	align-content: center;
	margin-bottom: 20px;
}
h1{
	text-align: center;
	color:rgb(226, 220, 220);
	font-family: sans-serif;
	text-transform: uppercase;
}
.container{
	box-sizing: border-box;
	width: 900px;
	padding: 8px;
	/* border: 1px solid #ccc;
	box-shadow: 0 2px 2px #aaa; */
	margin: 10px;
	background: rgba(0, 0, 0, .7);
	border-radius: 10px;
	box-shadow: 0 15px 50px rgba(0, 0, 0, .7);
}
.usercontainer{
	max-width: 800px;
}
 ul{
	 list-style: none;
 }
 a{
	 text-decoration: none;
	 color:rgb(226, 220, 220);
	 font-family: sans-serif;
     text-align: center;
     padding-bottom: 10px;
 }
 li{
	color:rgb(226, 220, 220);
	font-family: sans-serif;
 }
 </style>


