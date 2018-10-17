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
	  	<div id="blog">
	  		<div class="highLightWrap">
		  			  		
		  			<nuxt-link
							v-for="(item,index) in dataHighlight"
		          :key="index"
		          :to="`/blog/${item._id}`"
		          :class="`grid${index+1}`"
		          :style="`background-image: url('${item.Thumbnail}')`"
		        >	
		        	<div id="descHighLight">		
			  				<p id="titleHighLight">{{item.Title}}</p>
			  				<p id="dateHighLight">{{item.createdAt}}</p>
			  			</div>
		  			</nuxt-link>

		  	</div>

		  	<div id="border">
		      <p id="borderText">LATEST POSTS</p>
		      <div id="borderLine"></div>
		    </div>
	      <div id="postWrapper">

	        <nuxt-link
	          v-for="(item,index) in dataAll"
	          :key="index"
	          :to="`/blog/${item._id}`"

	        >
	          <div class="post">
	            <div 
	            	class="thumbnail" 
	            	:style="`background-image: url('${item.Thumbnail}')`"
	            >
	            	
	            </div>
	            <div class="description">
	              <div class="titleWrap">
	                <p class="darkBlue h3 title">{{ item.Title }}</p>
	                <p class="darkBlue date">{{ item.createdAt }}</p>
	            </div>
	            </div>
	          </div>
	        </nuxt-link>

	      </div>
	      <div id="borderLineBottom"></div>
	    </div>
	  </div>

	</section>
</template>

<script>
export default{
	mounted() {
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
	},
	data() {
    return {
    	dataHighlight: '',
      dataAll: ''
    }
  },
  methods: {

  },
  created() {
    function loadJSON(callback) {   

      var xobj = new XMLHttpRequest();
      xobj.overrideMimeType("application/json");
      xobj.open('GET', 'blog.json', true); 
      xobj.onreadystatechange = function () {
        if (xobj.readyState == 4 && xobj.status == "200") {
          try {
            var data = JSON.parse(xobj.responseText);
          } catch(err) {
            console.log('error')
            return;
          }
          callback(data);
        }
      };
      xobj.send(null);  
    }
    var self = this;
    loadJSON(function(data) {
      self.dataHighlight = data.data.slice(0,3);
      self.dataAll = data.data.slice(3);
      console.log(self.dataHighlight);
    });

    window.addEventListener("resize", function() {
      console.log('resize!');
      if (window.innerWidth > 767) {
        document.getElementById('nav').style.left = '50%';
      }

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

div#blog{
  padding: 100px 200px 75px;
  display: flex;
  flex-wrap: wrap;
}

.grid1 { 
	grid-area: main;
	height: 500px;
}
.grid2 { grid-area: right; }
.grid3 { grid-area: bottom; }

div.highLightWrap{
	flex: 0 0 100%;
	display: grid;
	background-color: lightgreen;
	grid-template-areas: 
		'main main right'
		'main main bottom';
	grid-gap: 10px;
	margin-bottom: 3rem;
	max-width: 992px;
}

div.highLightWrap a{
	border: 1px solid black;
	text-align: center;
  position: relative;
}

div.highLightWrap a div#descHighLight{
	position: absolute;
	bottom: 0;
	width: 100%;
	border: 1px solid red;
}

div.highLightWrap a div#descHighLight p{
	padding: 1rem;
	text-align: left;
	border: 1px solid yellow;
	color: white;
	overflow: hidden;
	text-overflow: ellipsis;
	white-space: nowrap;
}

div.highLightWrap a.grid1 div#descHighLight p:first-child{
	padding: 2rem 1rem;
	font-size: 1.5rem;
	text-align: left;
	border: 1px solid yellow;
}

div#border{
	position: relative;
	flex: 0 0 100%;
	text-align: center;
}

p#borderText{
	display: inline;
	background-color: white;	
	text-align: center;
	z-index: 999;
	padding: 0 10px;	
	flex: 0 0 100%;
}

div#borderLine, div#borderLineBottom{
	flex: 0 0 100%;	
	height: 2px;
	background-color: #EEEEEE;
	margin-top: -12px;
	margin-bottom: calc(2rem + 12px);
}

div#borderLineBottom{
	margin-bottom: 0;
	margin-top: 2rem;
}

div#postWrapper{
  width: 100%;
  max-width: 992px;
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
  background-size: cover;
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

@media screen and (min-width: 1366px) {
	div#blog{
    justify-content: center;
  }
}

@media (min-width: 992px) and (max-width: 1199px) {
	div#blog{
    padding: 150px 150px 75px
  }
}	

@media (min-width: 768px) and (max-width: 991px) {
	div#blog{
    padding: 150px 100px 75px
  }

  div#blog p{
    font-size: 1.25rem;
  }

  div#blog div.post{
    height: 150px;
  }
}

@media screen and (max-width: 767px) {
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

  div#blog{
  	padding: 75px 30px;
  }

  .grid1 { 
		grid-area: main;
	}
	.grid2 { grid-area: right; }
	.grid3 { grid-area: bottom; }

	div.highLightWrap{
		grid-template-areas: 
			'main'
			'right'
			'bottom';
	}

	div.highLightWrap a{
	  height: 300px;
	}

  div#blog div.thumbnail, div#blog div.description{
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

  div#borderLineBottom{
		margin-top: 0;
	}
}

</style>