<template>
    <header>
        <nav class="black">
            <div class="logo">LOGO</div>
            <ul>
                <li><nuxt-link to="/">Home</nuxt-link></li>
                <li><nuxt-link to="/user">User</nuxt-link></li>
                <li><nuxt-link to="/">About</nuxt-link></li>
                <li><nuxt-link class="active" to="/">Login</nuxt-link></li>
            </ul>
        </nav>
        <section class="sec1"></section>
    </header>
</template>

<style scoped>
nav{
    /* position:fixed; */
    top: 0;
    left: 0;
    width: 100%;
    height: 60px;
    padding: 10px 100px;
    box-sizing: border-box;
    transition: .3s;
}
nav.black{
    background: rgba(0, 0, 0, 0.8);
    height: 100px;
    padding: 10px 100px;
}
nav .logo{
    padding: 22px 20px;
    height: 80px;
    float: left;
    font-size: 24px;
    transition: .3s;
}
nav.black .logo{
    color: #fff;
}
nav ul{
    list-style: none;
    float:right;
    margin: 0px;
    padding: 0px;
    display: flex;
}
nav ul li{
    list-style: none;
}
nav ul li a{
    line-height: 80px;
    color:  #151515;
    padding: 12px 30px;
    text-decoration: none;
    text-transform: uppercase;
    transition: .3s;
}
nav.black ul li a{
    color: #fff;
}
nav ul li a:focus{
    outline: none;
}
nav ul li a.active{
    background: #E2472F;
    color: #ffffff;
    border-radius: 6px;
}
</style>

