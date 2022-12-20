<template>
  <div>
    <div class="body">
      <div style="padding-top:90px; ">
        <div class="container">
          <div class="row" >
            <div class="col-md-6">
             <div style="padding-top:90px; ">
              <div style="color: #81b622;padding-left:40px;">
                <h5>Hi , my name is</h5>
              </div>
              <div style="color: white; font-weight:bold; font-size:55px; padding-left:40px;">
                <p>Nisha Pandey.</p>
              </div>
              <div style="color: grey;font-weight:bold; font-size:45px;padding-left:40px;">
                <p class="reveal-text">I'm a Front-End Developer</p>
              </div>
            
              <div style="margin: 10px 10px 10px 10px; padding-left:40px;">
                <div class="box">
                  <button><span>Contact Me</span></button>
                </div>
                
              </div>
             </div>
            </div>
            <div class="col-md-6">
              <img src="../assets/me-removebg-preview.png" alt="" style="width:70%;">
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IntroComponent",
};
</script>

<style  scoped>

@supports (-webkit-background-clip: text) or (background-clip: text) {
  .reveal-text {
      color: transparent;
      -webkit-background-clip: text;
      background-clip: text;
      background-image: url("https://raw.githubusercontent.com/WebDevSimplified/css-challenges/master/Animated%20Text%20Reveal/reveal_background.jpg");
      background-repeat: repeat-x;
      animation: reveal-background 8s ease-in-out infinite;
      animation-fill-mode: forwards;
  }
}

@keyframes reveal-background {
  0% {
      background-size: 0px;
      background-position-y: 0%;
  }
  10% {
      background-size: 30px;
      background-position-y: 0%;
  }
  35%, 45% {
      background-position-y: 100%;
  }
  70% {
      background-size: 30px;
      background-position-y: 0%;
  }
  100% {
      background-size: 200px;
  }
}

/* Background Styles Only */

*{
  box-sizing: border-box
}
.box{
  width: 600px;
  margin: auto;
  padding-top: 20px;
  overflow: hidden;
  height: 100%
}

.box button{
  height:60px;
  width: 250px;
  line-height: 60px;
  background: transparent;
  border: 3px solid #fff;
  border-radius: 10px;
  margin: 10px;
  font-size: 16px;
  color: #fff;
  text-transform: uppercase;
  cursor: pointer;
  float: left;
  display: block;
  position: relative;
  overflow: hidden
}

.box button span{
  width: 100%;
  display: block;
  text-align: center;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 2;
  transition: all 0.1s ease 0.3s
}

button:hover span{color: #fff}



button:first-child{
  color: #81b622;
  border-color: #81b622;
}

button:first-child:before{
  content: "";
  display: block;
  position: absolute;
  top: 50%;
  left: 300px;
  width: 30px;
  height: 30px;
  background: #81b622;
  border-radius: 50%;
  transform: translateY(-50%);
}

button:first-child:hover:before{
  animation: hover-one 1s ease forwards
}

@keyframes hover-one{
  0%{
    top: 50%;
    left: 300px;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    transform: translateY(-50%);
    opacity: 0
  }
  25%{
    top: 50%;
    left: 0;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    transform: translateY(-50%);
    opacity: 0.7
  }
  50%{
    top: 0;
    left: 0;
    width: 25%;
    height: 100%;
    border-radius: 0;
    transform: translateY(0);
    opacity: 1
  }
  100%{
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 0;
    transform: translateY(0);
  }
}

@media (max-width: 620px){
  
  .box{width: 100%}
  
  .box button{
    float: none;
    margin: 20px auto;
  }
}
</style>
