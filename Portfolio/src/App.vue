<script setup>

import TheHeader from '@/components/TheHeader.vue'

</script>

<template>
  <TheHeader></TheHeader>
  <main class="main">
    <div class="hero">
      <img src="./assets/background.jpg" alt="Background Image" class="hero__image">
      <div class="hero__container"> 
        <div class="hero__info">
          <div class="hero__info__bar"></div>  
          <p class="hero__title">Front-End Developer</p>
          <p class="hero__text">I am a Developer, a Coder, and an Artist, but before all that I'm a Problem Solver. I enjoy doing challenging projects that require mixing my artistic side and my technical knowledge.</p>
          <p class="hero__title">My workflow & Approach</p>
          <p class="hero__text">My Workflow differs from project to project but what stays the same is my approach. I try to understand the project and its needs and while doing so I determine the best tools to built it. <br><br> For one project I might go with Test Driven Development, Scrum Board, React, and Type Script and for another just a simple sketch on a paper and vanilla JS.</p>
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss">

  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;700&display=swap');

  //RESETS
  html {
    box-sizing: border-box;
    
    font-family: 'Poppins', sans-serif;
  }

  *, *:before, *:after {
    box-sizing: inherit;
  }

  body {
    background-color: #191919;
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
  }
  a, li, h1, h2, p {
    text-decoration: none;
    margin: 0;
    padding: 0;
    z-index: 9998;
  }

  ul {
    display: inline;  
    margin: 0;
    padding: 0;
  }
  li {
    display: inline;
    list-style-type: none;
    margin: 0;
    padding: 0; 
  }

  .main {
    width: 100%;
  }

  .hero {
    overflow: hidden;
    position: relative;
    width: 100%;
    height: 80vh;
    .hero__image {
      position: absolute;
      width: 100%;
      opacity: .2;
      top: 0;
      left: 0;
      z-index: 999;
    }

    .hero__container {
      position: relative;
      background: linear-gradient(0deg, rgba(25,25,25,1) 0%, rgba(25,25,25,.7) 15%, rgba(25,25,25,.7) 99%, rgba(25,25,25,1) 100%);

      width: 100%;
      height: 100%;
      z-index: 9998;

      .hero__info {
        position: relative;
        width: 50%;
        height: 100%;
        padding: 4rem;

        .hero__title {
          color: #c99f7c;
          font-size: 3rem;

          margin-top: 4rem;
        }

        .hero__text {
          color: #EEEEEE;
          
          border-left: .2rem solid #c99f7c;
          
          padding-left: 1rem;
          margin-left: 1.15rem;
          margin-top: 1rem;

        }
      }
    }
}

</style>
