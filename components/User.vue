<template>
	<article>
		<section>
			<div class="container">
				<div class="usercontainer">
					<nuxt-link :to="'/user/' + id">
						<div>
							<ul>
								<li><b>Name:</b> {{ name }}</li>
								<li><b>Email:</b> {{ email }}</li>
								<li><b>Phone:</b> {{ phone }}</li>
								<li><b>Website:</b> {{ website }}</li>
								<li><b>Company:</b> {{ companyname }}<br><b>CatchPhrase:</b> {{ companycatchPhrase }}<br><b>Bs:</b> {{ companybs }}<br></li><br>             <li><u>Click to view user details!</u></li>
							</ul>
							<br>
						</div> 
					</nuxt-link>           
				</div>
			</div>
		</section>
	</article>
</template>

<script>
	export default {
		props: ['name', 'email', 'phone', 'website', 'companyname', 'companycatchPhrase', 'companybs', 'id']
	}
</script>
<style scoped>
.container{
	box-sizing: border-box;
	width: 450px;
	padding: 8px;
	/* border: 1px solid #ccc;
	box-shadow: 0 2px 2px #aaa;*/
	margin: 10px;
	/* transform: translate(-50%,-50%); */
	/* width: 900px; */
	background: rgba(0, 0, 0, .7);
	border-radius: 10px;
	box-shadow: 0 15px 50px rgba(0, 0, 0, .7);
}
.usercontainer{
	max-width: 440px;
}
 ul{
	 list-style: none;
 }
 a{
	 text-decoration: none;
	 color:rgb(226, 220, 220);
	 font-family: sans-serif;
 }
 a:focus{
	 outline: none;
 }
</style>
