<template>
  <section class="user">
    <ul>
      <h1>Latest posts</h1>
      <li>
        <div class="date">
          <h3>Nov<br><span>23</span></h3>
        </div>
        <a href="#">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
          </p>
        </a>
      </li>
      <li>
        <div class="date">
          <h3>Nov<br><span>23</span></h3>
        </div>
        <a href="#">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
          </p>
        </a>
      </li>
      <li>
        <div class="date">
          <h3>Nov<br><span>23</span></h3>
        </div>
        <a href="#">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
          </p>
        </a>
      </li>
      <li>
        <div class="date">
          <h3>Nov<br><span>23</span></h3>
        </div>
        <a href="#">
          <p>
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
          </p>
        </a>
      </li>
    </ul>
  </section>
</template>

<style scoped>
body{
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}
section{
  width:100%;
  height: 100vh;
  background-image: url('https://cdn-images-1.medium.com/max/1330/1*CsDgB2D8KIetB_e37t3n_A.jpeg');
  background-size: cover;
  background-position: center;
}
ul{
  margin: 0;
  padding: 20px;
  position:absolute;
  top: 60%;
  left: 50%;
  transform: translate(-50%,-50%);
  width: 900px;
  background: rgba(0, 0, 0, .7);
  border-radius: 10px;
  box-shadow: 0 15px 50px rgba(255, 255, 255, 0.5);
}
h1{
  color: #ffffff;
  margin: 0 0 10px;
  padding: 0 0 10px;
  font-size: 24px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.5);
}
ul li{
  position: relative;
  list-style: none;
  padding: 4px;
  border-radius: 4px;
  border-bottom: 1px solid rgba(255, 255, 255, 0.4);
}
ul li a{
  color: #ffffff;
  text-decoration: none;
  display: block;
  padding-top:20px;
  padding-bottom: 20px;
  padding-left: 140px;
}
ul li h3{
  position: relative;
  z-index: 2;
  margin-top: -6px;
  font-size: 16px;
  color: #ffffff;
  line-height: 36px;
}
ul li h3 span{
  color: #324d5b;
  font-size: 36px;
}
ul li .date{
  position: absolute;
  /* padding-top:20px; */
  padding-bottom: 20px;
  top: 0;
  left: 0;
  width: 100px;
  text-align: center;
}
ul li .date:before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 0;
  border-top: 22px solid #e2574c;
  border-bottom: 50px solid #e4e7e7;
  z-index: 1;
  border-radius: 5px;
}
ul li .date p{
  font-size: 18px;
}
</style>
