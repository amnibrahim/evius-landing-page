<template>
  <div>
    <nuxt/>
  </div>
</template>

<style>
*{
  padding: 0;
  margin: 0;
  text-shadow: transparent 0 0 0, rgba(0,0,0,.68) 0 0 0 ;
  box-sizing: border-box;
  font-family: 'Raleway', sans-serif;
}

/* latin-ext */
@font-face {
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  src: local('Raleway'), local('Raleway-Regular'), url(https://fonts.gstatic.com/s/raleway/v12/1Ptug8zYS_SKggPNyCMIT5lu.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  src: local('Raleway'), local('Raleway-Regular'), url(https://fonts.gstatic.com/s/raleway/v12/1Ptug8zYS_SKggPNyC0ITw.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}

html{
  font-size: 14px;
  color: #2E466E;
}

body{
  font-family: 'Raleway', sans-serif;
  margin : 0;
  padding: 0;
}

.h1, .h2, .h3, .h4, .h5, .h6, h1, h2, h3, h4, h5, h6, p{
  margin-bottom: 0;
  margin-top : 0;
  line-height: 1.5;
}

h1{
  font-size: 4rem;
}

h2{
  font-size: 1.5rem;
}

h3{
  font-size: 1rem;
}

h4{
  font-size: 0.875rem;
}

h5{
  font-size: 0.75rem;
}

h6{
  font-size: 0.625rem;
}

dl, ol, ul{
  margin-bottom: 0;
}

.h1{
  font-size: 4rem;
}

.h2{
  font-size: 2.25rem;
}

.h3{
  font-size: 1.75rem;
}

.h4{
  font-size: 0.875rem;
}

.h5{
  font-size: 0.875rem;
}

.h6{
  font-size: 0.625rem;
}

.fw-3{
  font-weight: 300
}

.fw-4{
  font-weight: 400
}


.fw-5{
  font-weight: 500
}


.fw-6{
  font-weight: 600
}

.fw-7{
  font-weight: 700
}

.flex-center{
  display: flex;
  align-items: center;
  justify-content: center;
}

p{
  font-size: 1rem;
  line-height: 24px;
  color: #0A1743;
  letter-spacing: 1px;
}

a{
  text-decoration: none;
}

.button{
  text-decoration: none;
  padding: 0.75rem 1.25rem;
  letter-spacing: 1.5px; 
  border: 0;
}

.title{
  text-align: center;
  margin-bottom: 1.5rem;
  flex: 0 0 100%;
}

.separatorWrapper{
  height: 3px;
  display: flex;
  justify-content: center;
  flex: 0 0 100%;
  margin-bottom: 100px;
}

.separator{
  width: 100px;
}

/*----------------------------*/

.black{
  color: #000000;
}
.bgblack{
  background: #000000;
}

.white{
  color: #FFFFFF;
}
.bgwhite{
  background: #FFFFFF;
}

.darkBlue{
  color: #0A1743;
}
.bgdarkBlue{
  background: #0A1743;
}

.blue{
  color: #1C3997;
}
.bgblue{
  background: #1C3997;
}

.grey{
  color: #EEEEEE;
}
.bggrey{
  background: #EEEEEE;
}

.cyan{
  color: #A3F3FD;
}
.bgcyan{
  background: #A3F3FD;
}

</style>