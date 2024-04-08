<script setup>

import TheHeader from '@/components/TheHeader.vue'
import PostCard from '@/components/ProjectCard.vue'
import Overlay from '@/components/Overlay.vue'

import projectPicWordle from '@/assets/Projects/wordle-screenshot.png'
import projectPicCafeLotte from '@/assets/Projects/Cafe Lotte Screenshot.png'
import projectPicCurrency from '@/assets/Projects/Curency-Converter.png'
import projectPicDDC from '@/assets/Projects/DDC Remake Screenshot.png'
import projectPicEplodedView from '@/assets/Projects/Exploded View Screenshot.png'
import projectPicGalleryVJ from '@/assets/Projects/Gallery Website homepage Screeshot.png'
import projectPicGalleryReact from '@/assets/Projects/Gallery Website Screeshot.png'
import projectPicTODOs from '@/assets/Projects/TODOs Screenshot.png'
import projectPicPS from '@/assets/Projects/ps-screenshot.png'
import projectPicOldPortfolio from '@/assets/Projects/old-portfolio-screenshot.png'
import projectPicDPLP from '@/assets/Projects/dp-lp-screenshot.png'
import projectPicAdviceGen from '@/assets/Projects/advice-generator-app.png'
import projectPicICDF from '@/assets/Projects/interactive-card-details-form.png'


import componentPicIR from '@/assets/Projects/interactive-rating.png'
import componentPicDS from '@/assets/Projects/fylo-data-storage.png'
import componentPicProductPre from '@/assets/Projects/product-preview-card.png'
import componentPicPricing from '@/assets/Projects/pricing-component-with-toggle.png'


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
        <div class="hero__action">
          <div onclick="window.location='#projects'" class="hero__btn">
            <p class="hero__btn__p">To The Projects</p>
          </div>
        </div>
      </div>
    </div>

    <div id="projects" class="projects">
      <h1 class="projects__title">Projects</h1>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/Wordle-Game/" :image="projectPicWordle" title="Wordle Game with Vue"></PostCard>
        <PostCard href="" :image="projectPicCafeLotte" title="Cafe lotte"></PostCard>
        <PostCard href="" :image="projectPicDDC" title="Dance School Website"></PostCard>
      </div>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/Exploded-View-Animation-Test-v2/" :image="projectPicEplodedView" title="Portfolio with Exploded View"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/Currency-Converter/" :image="projectPicCurrency" title="Currency Converter with API + Dark Mode"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/TODOs/" :image="projectPicTODOs" title="TODOs App with Vanila JS"></PostCard>
      </div>
      <div class="projects__row">
        <PostCard href="" :image="projectPicGalleryVJ" title="Gallery Website"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/gallery-website-react/" :image="projectPicGalleryReact" title="Gallery Website with React"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/playstation-website-clone/" :image="projectPicPS" title="Play Station Website Clone"></PostCard>
      </div>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/Portfolio-v2/" :image="projectPicOldPortfolio" title="Personal Portfolio"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/simple-landing-page-dance-program/" :image="projectPicDPLP" title="Dance Program Landing Page"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/advice-generator-app-main/" :image="projectPicAdviceGen" title="Advice generator app"></PostCard>
      </div>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/interactive-card-details-form-main/" :image="projectPicICDF" title="Interactive card details form"></PostCard>
      </div>
  
      <h1 class="projects__title">Components</h1>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/interactive-rating-component-main/" :image="componentPicIR" title="Interactive rating component"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/fylo-data-storage-component-master/" :image="componentPicDS" title="Data Storage Display component"></PostCard>
        <PostCard href="https://barbodgarsha.github.io/product-preview-card-component/" :image="componentPicProductPre" title="Product Preview Card component"></PostCard>
      </div>
      <div class="projects__row">
        <PostCard href="https://barbodgarsha.github.io/pricing-component-with-toggle-master/" :image="componentPicPricing" title="Pricing with toggle component"></PostCard>
      </div>
    </div>
    
    <Overlay>
      <div class="project-info">
        <img class="project-info__img" :src="projectPicAdviceGen" alt="">
      </div>
    </Overlay>
  </main>
</template>

<style lang="scss">

  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;700&display=swap');

  //RESETS
  html {
    box-sizing: border-box;
    scroll-behavior: smooth;

    font-family: 'Poppins', sans-serif;
  }
  ::-webkit-scrollbar {
    width: 0;  /* Remove scrollbar space */
    background: transparent;  /* Optional: just make scrollbar invisible */
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
    height: 88vh;
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

      display: flex;

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

      .hero__action {
        display: flex;
        justify-content: center;
        align-items: center;

        width: 50%;
        .hero__btn {
          cursor: pointer;

          background-color: #D65A31;
          box-shadow: 0px 0px 20px 2px #D65A31;
          border-radius: 15rem;
          padding: 2rem 4rem;

          transition-duration: 100ms;
          transition-timing-function: ease-in;
          .hero__btn__p {
            color: #191919;
            font-size: 2rem;
            font-weight: 500;
            transition-duration: 100ms;
            transition-timing-function: ease-in;
          }
        }
        .hero__btn:hover {
          box-shadow: 0px 0px 30px 3px #D65A31;
          .hero__btn__p {
            color: #EEEEEE;
          }
        }
      }
    }
  }

  .projects {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;

    .projects__title {
      color: #EEEEEE;
      padding: 1rem;
    }

    .projects__row {  
      padding: 1rem 0;
      display: flex;
      justify-content: space-evenly;
      flex-wrap: wrap;
    }
  }

  .project-info {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;

    width: 100%;
    height: 100%;

    .project-info__img {
      width: 100%;
      border-radius: 9px;
    }
  }
</style>
