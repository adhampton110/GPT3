<script setup>
  import Header from './layouts/Header/Header.vue';
  import GPTGroupData from './data/GPTGroupData.json';
  import FutureData from './data/FutureData.json';
  import GPT3Group from './components/GPT3Group.vue';
  import GradientLine from './components/GradientLine.vue';
  import FutureGroup from './components/FutureGroup.vue';
  import Footer from './layouts/Footer/Footer.vue';
  import OrangeButton from './components/OrangeButton.vue';
</script>

<template>
  <!-- Header -->
  <Header/>

  <!-- Hero -->
  <section class="hero">
    <div class="content">
      <h1>Let's Build Something amazing with GPT-3 OpenAI</h1>
      <p>
        Yet bed any for travelling assistance indulgence unpleasing. Not thoughts all exercise blessing. Indulgence way everything joy alteration boisterous the attachment. Party we years to order allow asked of.
      </p>
      <div class="getting-started">
        <input placeholder="Your Email Address" type="text">
        <button>Get Started</button>
      </div>
      <div class="requested-access">
        <img src="./assets/people.png" alt="people">
        <p>1,600 people requrested access a visit in last 24 hours</p>
      </div>
    </div>
    <img src="./assets/ai.png" width="670px" height="700px" alt="ai">
  </section>

  <!-- Affiliate Icons -->
  <div class="affiliates">
    <img src="./assets/google.png" alt="">
    <img src="./assets/slack.png" alt="slack">
    <img src="./assets/atlassian.png" alt="atlassian">
    <img src="./assets/dropbox.png" alt="dropbox">
    <img src="./assets/shopify.png" alt="shopify">
  </div>

  <!-- What is GPT3 -->
  <section class="gpt3">
    <div class="gpt3-top-wrapper">
      <GradientLine/>
      <div class="gpt3-top">
        <h3>What is GPT-3</h3>
        <p>
          We so opinion friends me message as delight. Whole front do of plate heard oh ought. His defective nor convinced residence own. Connection has put impossible own apartments boisterous. At jointure ladyship an insisted so humanity he. Friendly bachelor entrance to on by.
        </p>
      </div>
    </div>
    <div class="gpt3-middle">
      <h2>The possibilities are beyond your imagination</h2>
      <p>Explore the Library</p>
    </div>
    <div class="gpt3-bottom">
      <GPT3Group v-for="obj in GPTGroupData" :title="obj.title" :msg="obj.message"/>
    </div>
  </section>

  <!-- Future is Now -->
  <section class="future">
    <div class="future-left">
      <h2>The Future is Now and You Just Need To Realize It. Step into Future Today & Make it Happen.</h2>
      <p>Request Early Access to Get Started</p>
    </div>
    <div class="future-right">
      <FutureGroup v-for="obj in FutureData" :title="obj.title" :msg="obj.message"/>
    </div>
  </section>

  <!-- Register -->
  <div class="register">
    <div>
      <p>Request Early Access to Get Started</p>
      <h3>Register today & start exploring the endlesss possibilities</h3>
    </div>
    <button class="getStarted">Get Started</button>
  </div>

  <!-- Footer -->
  <section class="footer">
    <h1>Do you want to step in to the future before others</h1>
    <button>Request Early Access</button>
    <Footer/>
  </section>
  
</template>
