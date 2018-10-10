<template>
  <section class="container">
    <div id="nav">
    <div class="menu menuLogo">
      <img src="~/assets/img/logo.png">
    </div>
    <div class="menu">

      <a class="fw-6 h5 darkBlue" href="#service" type="scroll">
        <img src="~/assets/img/service.png" class="menuIcon">
        SERVICE
      </a>
      <a class="fw-6 h5 darkBlue" href="#solution" type="scroll">
        <img src="~/assets/img/project.png" class="menuIcon">
        PROJECT
      </a>
      <a class="fw-6 h5 darkBlue" href="#work" type="scroll">
        <img src="~/assets/img/work.png" class="menuIcon">
        WORK
      </a>
      <a class="fw-6 h5 darkBlue" href="#blog" type="scroll">
        <img src="~/assets/img/blog.png" class="menuIcon">
        BLOG
      </a>
      <a class="fw-6 h5 darkBlue" href="#contact" type="scroll">
        <img src="~/assets/img/contact.png" class="menuIcon">
        CONTACT
      </a>
    </div>
  </div>

  <div id="menuHamburger">
    <div class="bgdarkBlue"></div>
    <div class="bgdarkBlue"></div>
    <div class="bgdarkBlue"></div>
  </div>

  <div id="contentWrapper">

    <div id="hero">

      <div id="heroTitle">
        <span class="cyan fw-7" id="heroAphos"><i>''</i></span>
        <p class="h1 fw-7" id="heroTitleText">We bring<br>emotion to your product</p>
        <p class="fw-5" id="heroBodyText">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
        <a class="button bgdarkBlue white fw-6" target="_blank" href="contact">CONTACT US</a>
        <p id="heroCornerText"><span class="bgcyan">Lorem ipsum<br>dolor sit amet consectetur</span></p>
        <div id="heroArrow">
          <a href="#service" type="scroll">
          <span>&#9472;&#9472;&#9472;&#9472;&#9472;&#9472;&#9472;&#9472;&#9472;&#9654;</span>
          </a>
        </div>
      </div>
    </div>

    <div id="service">
      <div class="title">
        <p class="darkBlue h2">Services</p>
      </div>
      <div class="separatorWrapper">
        <div class="separator bgcyan"></div>
      </div>
      <div id="serviceGrid">
        <div class="gridCell">
          <p><span class="h3">Modern <br>technology</span>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation.</p>
          <object type="image/svg+xml" data="svg/undraw_real-time_sync_o57k.svg" id="grid1"></object>
        </div>
        <div class="gridCell">
          <object type="image/svg+xml" data="svg/undraw_Devices_e67q.svg" id="grid1"></object>
          <p><span class="h3">Data <br>driven UI/UX</span>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod 
          tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation.</p>
        </div>
        <div class="gridCell">
          <p><span class="h3">Flexible <br>and scalable</span>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
          tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
          quis nostrud exercitatio.</p>
          <object type="image/svg+xml" data="svg/undraw_tabs_jf82.svg" id="grid1"></object>
        </div>
      </div>
    </div>

    <div id="solution">
      <div class="title">
        <p class="darkBlue h2">Solutions</p>
      </div>
      <div class="separatorWrapper">
        <div class="separator bgcyan"></div>
      </div>
      <div id="solutionGrid">
        <div class="gridSolCell">
          <p class="fw-6">Online Store</p>
          <img src="~/assets/img/aa.png">
        </div>
        <div class="gridSolCell">
          <p class="fw-6">SaaS</p>
          <img src="~/assets/img/bb.png">
        </div>
        <div class="gridSolCell">
          <p class="fw-6">Social Network</p>
          <img src="~/assets/img/cc.png">
        </div>
      </div>
      <div id="demo">
        <div id="demoWrapper">
          <input type="text" name="" placeholder="Email">
          <a class="button bgdarkBlue white" href="mailto:mamamia@evius.com">REQUEST A DEMO</a>
        </div>
      </div>
    </div>

    <div class="bggrey" id="work">
      <div id="workTitle">
        <div class="title">
          <p class="darkBlue h1 fw-7">
            <span>Our</span>
            <span>Latest</span> 
            <span>Work</span>
          </p>
        </div>
        <div class="separatorWrapper">
          <div class="separator bgcyan"></div>
        </div>
      </div>
      <div id="sliderWrapper">
        <div id="slider">
          <img name="slider">
        </div>
      </div>
    </div>

    <div id="blog">
      <div class="title">
        <p class="darkBlue h2">Blog</p>
      </div>
      <div class="separatorWrapper">
        <div class="separator bgcyan"></div>
      </div>
      <div id="postWrapper">
        <a href="blog">
          <div class="post">
            <div class="thumbnail">
              <img src="~/assets/img/t.png">
            </div>
            <div class="description">
              <div class="titleWrap">
                <p class="darkBlue h3 title">Top 6 Software Development Methodologies</p>
                <p class="darkBlue date">May 16, 2018</p>
              </div>
            </div>
          </div>
        </a>
        <a href="blog">
          <div class="post">
            <div class="thumbnail">
              <img src="~/assets/img/u.jpg">
            </div>
            <div class="description">
              <div class="titleWrap">
                <p class="darkBlue h3 title">Git and Interactive Patch Add</p>
                <p class="darkBlue date">May 16, 2018</p>
              </div>
            </div>
          </div>
        </a>
        <a href="blog">
          <div class="post">
            <div class="thumbnail">
              <img src="~/assets/img/v.jpg">
            </div>
            <div class="description">
              <div class="titleWrap">
                <p class="darkBlue h3 title">A beginner's Introduction to Working with Redux in React</p>
                <p class="darkBlue date">May 16, 2018</p>
              </div>
            </div>
          </div>
        </a>
        <div class="post" id="viewWrapper">
          <div id="viewButton">
            <button class="button">VIEW ALL</button>
          </div>
        </div>
      </div>
    </div>

    <div id="contact">
      <div id="contactus">
        <div class="contactGrid">
          <p class="h3 white fw-6" id="contactTitle">Tell us what you want</p>
          <p class="white" id="contactBody">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud.</p>
          <a class="button bgcyan darkBlue fw-6" target="_blank" href="contact">CONTACT US&nbsp;<span> &#x279e;</span></a>
        </div>
      </div>
      <div id="careers">
        <div class="contactGrid">
          <p class="white h2 fw-6" id="careersTitle">Careers</p>
          <p class="white" id="careersBody">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          <p class="white fw-6" id="careersEmail">Send your email to &nbsp;&nbsp;&nbsp; mamamia@evius.com</p>
        </div>
      </div>
    </div>

    <div id="footer">
      <div id="footerWrapper">
        <p class="darkBlue fw-6">(C) Evius. 2018</p>
        <div id="socialIcon">
          <a href="#"><img src="~/assets/img/fb2.png"></a>
          <a href="#"><img src="~/assets/img/tw.png"></a>
          <a href="#"><img src="~/assets/img/ig.png"></a>
        </div>
      </div>
    </div>

  </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  mounted() {
    var i = 0;
    var images = [];
    var time = 2500;
    var timeout;

    images[0] = '/uu1.png';
    images[1] = '/uu2.png';
    images[2] = '/uu3.png';

    document.slider.src = images[i];

    setInterval(function(){

      if (i < images.length - 1) {
        i++;
        document.slider.src = images[i];
      }
      else {
        i = 0;
        document.slider.src = images[i];
      }

    },2500);

    var menu = 'hidden';

    document.getElementById('menuHamburger').addEventListener('click', function() {
      if (menu === 'shown') {
        
        document.getElementById('nav').style.left = 'calc(-1 * calc(100% - 56px))';
        document.getElementById('contentWrapper').style.filter = 'blur(0px)';
        document.getElementById('contentWrapper').style.pointerEvents = 'auto';
        menu = 'hidden';
        console.log(menu)
      }
      else{
        document.getElementById('nav').style.left = '0';
        document.getElementById('contentWrapper').style.filter = 'blur(10px)';
        document.getElementById('contentWrapper').style.pointerEvents = 'none';
        menu = 'shown';
        console.log(menu)
      }
    });

    window.addEventListener("resize", function() {

      console.log('resized');

      if (window.innerWidth > 767) {
        document.getElementById('nav').style.left = '50%';
      }

    });

    document.querySelectorAll('a[type^="scroll"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();

            console.log('scrolled')

            document.querySelector(this.getAttribute('href')).scrollIntoView({
                behavior: 'smooth'
            });
        });
    });
  }
}
</script>

<style scoped>

div#contentWrapper{
  transition: 0.1s;
}

div#nav{
  position: absolute;
  padding: 0 100px;
  width: 100%;
  max-width: 1366px;
  height: 36px;
  display: flex;
  justify-content: space-between; 
  margin-top: 20px;
  z-index: 999;
  transform: translateX(-50%);
  left: 50%;
}

div.menuHamburger, div#hero div#nav img.menuIcon,{
  display: none;
}

div.menu img{
  width: 24px;
  height: 24px;
}

div.menu img.menuIcon{
  display: none;
}

div.menu a{
  margin-left: 2rem;
}

div.menu{
  display: flex;
  align-items: center;
}

div.menu:first-child{
  width: 50%;
  justify-content: space-between;
}

div#hero{
  height: 100vh;
  display: flex;
  justify-content: center;
  position: relative;
}

div#heroTitle{
  width: calc(100% - 400px);
  position: absolute;
  bottom: calc(100vh / 4);
}

span#heroAphos{
  font-size: 15rem; 
  position: absolute;
  left: -60px;
  top: -60px;
  letter-spacing: -10px;
}

p#heroTitleText{
  margin-bottom: 1.5rem;
  letter-spacing: 1.5px;
  line-height: 80px;
  position: relative;
}

p#heroBodyText{
  width: 400px;
  margin-bottom: 4rem;
}

p#heroCornerText{
  position: absolute;
  right: 0;
  bottom: -0.75rem;
  text-align: right;
  line-height: 19px;
}

div#heroArrow{
  position: absolute;
  transform: rotate(90deg) translate(-100%, 300%) scale(0.5);
  left: 50%;
  bottom: -200px;
}

/*-----------------------*/

div#service{
  padding: 150px 200px 75px;
  display: flex;
  flex-wrap: wrap;
}

div#serviceGrid{
  width: 100%;
  padding: 0 150px;
}

div.gridCell{
  display: grid;
  grid: auto-flow dense / repeat(2, 50%);
  place-items: center;
  margin-bottom: 100px;
}

div#serviceGrid p span{
  line-height: 2rem;
  display: block;
  margin-bottom: 0.75rem;
}

div#serviceGrid p{
  padding: 0 2rem;
  max-width: 350px;
}

div#serviceGrid div:nth-child(odd) p{
  text-align: right;
  padding: 0 1.75rem;
}

object{
  width: 80%;
}

/*fallback svg
object#grid1{
  width: 200px;
  height: 164px;
  background-image: url(kiwi.png);
}*/

/*-----------------------*/

div#solution{
  padding: 75px 200px 150px;
  display: flex;
  flex-wrap: wrap;
}

div#solution div.separatorWrapper{
  margin-bottom: 50px;
}

div#solutionGrid{
  display: grid;
  grid: auto-flow dense / repeat(3, 33.333%);
  place-items: center;
  margin-bottom: 50px;
  text-align: center;
}

div#solutionGrid p{
  margin-bottom: 1.5rem;
}

div.gridSolCell{
  padding: 1.5rem;
}

div.gridSolCell img{
  width: 100%;
}

div#demo{
  display: none;
  flex: 0 0 100%;
  /*display: flex;*/
  justify-content: center;
}

div#demoWrapper input{
  padding: 0.6rem 1.25rem 0.6rem 1.25rem;
  width: 400px;
  margin-right: 1rem;
}

div#demoWrapper a{
  cursor: pointer;
}

/*-----------------------*/

div#work{
  padding: 0px 200px 0px;
  height: 100vh;
  display: grid;
  grid: auto-flow dense / repeat(2, 50%);
  place-items: center;
  /*margin-bottom: 50px;*/
}

div#workTitle{
  width: 100%;
}

div#workTitle div.title{
  margin-bottom: 3rem;
}

div#workTitle div.separatorWrapper{
  margin: 0;
}

div#workTitle div{
  text-align: left;
  justify-content: flex-start;
}

div#workTitle span{
  line-height: 4rem;
  display: block;
  margin-bottom: 2rem;
  letter-spacing: 5px;
}

div#slider{
  box-shadow: 0px 0px 25px -5px;
  border-radius: 10px;
}

div#slider img{
  width: 100%;
}

div#pointer{
  display: flex;
  justify-content: center;
  margin-top: 1.5rem;
}

div#pointer div{
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: #C4C4C4;
  cursor: pointer;
}

div#pointer div:nth-child(2){
  margin: 0 10px;
}

/*-----------------------*/

div#blog{
  padding: 150px 200px 75px;
  display: flex;
  flex-wrap: wrap;
}

div#postWrapper{
  width: 100%;
}

div.post{
  height: 200px;
  margin-bottom: 2rem;
}

div.thumbnail{
  width: 25%;
  height: 100%;
  float: left;
  overflow: hidden;
}

div.thumbnail img{
  /*width: 100%;*/
  height: 100%;
}

div.description{
  width: 75%;
  height: 100%;
  float: left;
  padding: 0 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 1px 1px 5px -2px;
}

div.titleWrap{
  width: 100%;
}

div.description p:first-child{
  margin-bottom: 1rem;
}

div.description p{
  text-align: left;
}

div#viewWrapper{
  display: flex;
  justify-content: center;
  height: auto;
}

div#viewButton{
  width: auto;
}

div#viewButton button:focus{
  outline: 0;
}

/*-----------------------*/

div#contact{

}

div#contactus{
  background: #14296C;
}
div#careers{
  background: #1C3997;
}

div#contactus, div#careers{
  width: 50%;
  height: 100%;
  float: left;
  display: flex;
  padding: 100px 0;
  align-items: center;
  justify-content: center;
}

div#contact div.contactGrid{
  width: 350px;
  height: 250px;
}

div#contact div p:first-child{
  letter-spacing: 2px;
}

p#contactBody{
  margin: 2rem 0 3rem;
}

p#careersBody{
  margin: 2rem 0;
}

div#careers div.separatorWrapper{
  margin: 2rem 0 0;
  justify-content: flex-start;
}

/*-----------------------*/

div#footer{
  display: flex;
  justify-content: center;
  padding: 50px 200px;
}

div#footerWrapper{
  width: 100%;
  max-width: 992px;
  display: flex;
  justify-content: space-between;
}

div#socialIcon img{
  height: 24px;
  margin-left: 12px;
}

</style>

<style scoped>
/* large desktops and up ----------- */
@media screen and (min-width: 1366px) {

  div#heroTitle{
    max-width: 992px;
    bottom: calc(100vh / 3);
  }

  div#service{
    justify-content: center;
  }

  div#serviceGrid{
    width: auto;
  }

  div#solution{
    justify-content: center;
  }

  div#solution div#solutionGrid{
    max-width: 992px;
  }

  div#workTitle{
    width: auto;
  }

  div#blog{
    justify-content: center;
  }

  div#blog div#postWrapper{
    max-width: 992px;
  }

}

/* tablets/desktops and up ----------- */
@media (min-width: 992px) and (max-width: 1199px) {

  div#hero{
    height: 66vh;
  }

  div#heroTitle{
    width: calc(100% - 300px);
    bottom: calc(100vh / 4);
  }

  div#service{
    padding: 0px 150px 75px;
  }

  div#serviceGrid{
    padding: 0 0px;
  }

  div#solution{
    padding: 75px 150px 150px;
  }

  div#work{
    height: 50vh;
    padding: 0px 150px 0px;
  }

  div#blog{
    padding: 150px 150px 75px
  }

}

/* Small devices (tablets, 768px and up) */
@media (min-width: 768px) and (max-width: 991px) {

  .button{
    font-size: 12px;
  }

  div#hero{
    height: 50vh;
  }

  div#heroTitle{
    width: calc(100% - 200px);
    bottom: calc(100vh / 10);
  }

  div#heroTitle p#heroTitleText{
      font-size: 3.2rem;  
      line-height: 60px;
  }

  div#service{
    padding: 75px 100px 75px;
  }

  div#serviceGrid{
    padding: 0 0px;
  }

  div#solution{
    padding: 0px 100px 150px;
  }

  div#solution div.gridSolCell{
    padding: 1rem;
  }

  div#solution div#demoWrapper input{
    width: 250px;
  }

  div#work{
    height: 50vh;
    padding: 0px 100px 0px;
  }

  div#work div.title p{
    font-size: 3.2rem;
  }

  div#blog{
    padding: 150px 100px 75px
  }

  div#blog p{
    font-size: 1.25rem;
  }

  div#blog div.post{
    height: 150px;
  }

  div#contact div.contactGrid{
    width: 300px;
  }

  div#contact div.contactGrid div.separatorWrapper{
    margin: 1.5rem 0 0;
  }

  div#contact div.contactGrid p#careersBody{
    margin: 1.5rem 0;
  }

}

/* Extra small devices (phones, up to 480px) */
@media screen and (max-width: 767px) {

  p{
    font-size: 12px;
  }

  .button{
    font-weight: 400;
  }

  .title{
    margin-bottom: 1rem;
  }

  .separatorWrapper{
    margin-bottom: 50px;
  }

  div#nav{
    position: fixed;
    left: calc(-1 * calc(100% - 56px));
    width: calc(100% - 56px);
    height: 100vh;
    transform: translateX(0);
    margin: 0;
    z-index: 999;
    background: rgba(10,23,67,0.9);
    transition: 0.5s; 
    padding: 0;
  }  

  div#nav div.menu{
    width: 100%;
    display: block;
    margin: 4rem 0.5rem;
  }

  div#nav div.menu.menuLogo:first-child{
    display: none;
  }

  div#nav img.menuIcon{
    display: inline;
    width: 12px;
    height: 12px;
    margin-right: 1.5rem;
  }

  div#nav a{
    margin-bottom: 3rem;
    display: block;
    color: white;
    font-weight: 400;
    letter-spacing: 1px;
  }

  div#menuHamburger{
    position: fixed;
      right: 16px;
      top: 18px;
      width: 24px;
      height: 24px;
      display: flex;
      justify-content: space-around;
      flex-direction: column;
      transition: 0.5s;
      z-index: 9999999;
  }

  div#menuHamburger div{
    width: 100%;
    height: 5px;
  }

  div#hero div#heroTitle{
    width: calc(100% - 75px);
    bottom: calc(100vh / 4);
    text-align: center;
  }

  div#hero div#heroTitle span#heroAphos{
    font-size: 11rem;
    left: 15px;
    top: -40px;
  }

  div#hero div#heroTitle p#heroTitleText{
    font-size: 2.25rem;
    line-height: 45px;
  }

  div#hero div#heroTitle p#heroBodyText{
    width: auto;
    margin-bottom: 3rem;
  }

  div#hero div#heroTitle p#heroCornerText{
    display: none;
  }

  div#service{
    padding: 50px 30px;
  }

  div#service div#serviceGrid{
    padding: 0;
  }

  div#service div#serviceGrid p span{
    font-size: 1rem;
    font-weight: 600;
  }

  div#service div#serviceGrid p span br{
    display: none;
  }

  div#service div#serviceGrid div.gridCell{
    margin-bottom: 32px;
    grid: auto-flow dense / repeat(1, 100%);
  }

  div#service div#serviceGrid div.gridCell p{
    padding: 0;
    text-align: left;
  }

  div#service div#serviceGrid div.gridCell object{
    display: none;
  }

  div#solution{
    padding: 50px;
  }

  div#solution div#solutionGrid{
    grid: auto-flow dense / repeat(1, 100%);
    margin-bottom: 16px;
  }

  div#solution div.gridSolCell{ 
    padding: 0;
    margin-bottom: 32px;
  }

  div#solution sdiv#solutionGrid p{
    margin-bottom: 0.75rem;
  }

  div#solution div#demoWrapper input, div#demoWrapper a{
    width: 100%;
    display: inline-block;
    margin-bottom: 1rem;
    text-align: center;
  }

  div#work{
    padding: 50px;
    height: auto;
    display: block;
  }

  div#work div#workTitle div.separatorWrapper{
    justify-content: center;
    margin-bottom: 50px;
  }

  div#work p{
    text-align: center;
    font-size: 2.25rem;
    font-weight: 400;
  }

  div#work div#workTitle span{
    line-height: 0;
    margin-bottom: 0;
    display: inline;
    letter-spacing: 1px;
  }

  div#work div.title{
    margin-bottom: 1rem;
  }

  div#work div#slider{
    box-shadow: 0px 0px 25px -10px;
  }

  div#blog{
    padding: 50px 30px;
  }

  div#blog div.thumbnail, div#blog div.description{
    width: 100%;
  }

  div#blog div.thumbnail img{
    width: 100%;
  }

  div#blog div.description{
    padding: 1rem;
    height: auto;
    margin-bottom: 32px;
    box-shadow: 0px 0px 5px -2px;
  }

  div#blog div.description div.titleWrap p{
    font-size: 1rem;
  }

  div#contact div#contactus, div#contact div#careers{
    width: 100%;  
    float: none;
    padding: 50px 50px 75px;
  }

  div#contact div.contactGrid{
    width: 100%;
    height: 100%;
  }

  div#contact span{
    display: none;
  }

  div#contact p#contactBody{
    margin: 1rem 0 2rem;
  }

  div#contact div#careers div.separatorWrapper{
    margin: 1rem 0 0;
  }

  div#contact p#careersBody{
    margin: 1rem 0;
  }

  div#footer{
    padding: 2rem 50px;
  }

  div#footerWrapper{
    display: block;
  }

  div#footerWrapper p{
    font-weight: 400;
    margin-bottom: 0.75rem;
  }

  div#footerWrapper img{
    height: 16px;
    margin-left: 0;
    margin-right: 12px;
  }
}
</style>