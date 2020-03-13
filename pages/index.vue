<template>
<body>
  <section class="hero is-fullheight has-background-black">
  <div class="hero-body">
    <div class="container">
    <div>
      <figure class="center">
        <nuxt-link to='/home'>
        <img src="~/assets/tobi-green.png" style="max-width: 512px" />
        </nuxt-link>
      </figure>
      <!-- <logo /> -->
      <!-- <h1 class="title">
        Tobi-Portfolio
      </h1> -->
      <h2 class="subtitle">
        My fast-expanding, amazing world of web programming
      </h2>
      <div class="links center">
      
        <a
          href="https://github.com/Oloruntobi1/"
          target="_blank"
          class="button--grey"
        >
          Visit my GitHub
        </a>

                <a
          href="https://twitter.com/lowcostbeans"
          target="_blank"
          class="button--grey"
        >
          Twitter
        </a>

                <a
          href="https://www.linkedin.com/in/balogun-tobi-4b6477169/"
          target="_blank"
          class="button--grey"
        >
          LinkedIn
        </a>
      </div>

      
      </div>
    </div>
  </div>
  </section>
  </body>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
   head () {
    return {
      title: 'An expanding world of web programming',
      meta: [
        { name: 'twitter:title', content: 'Links to lots of project you might love'},
        { name: 'twitter:description', content: 'Would always be worth the visit!'},
        // { name: 'twitter:image', content: 'https://i.imgur.com/UYP2umJ.png'},
        { name: 'twitter:card', content: 'summary_large_image'},
        {property: "og:title", content:"Askari Web projects"},
        {property: "og:description", content: "An avid web developer trove of personal projects."},
        {property: "og:image", content: "http://euro-travel-example.com/thumbnail.jpg"},
        {property: "og:url", content: "http://euro-travel-example.com/index.htm"}
      ]
    }
  },
}
</script>

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
} */

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.center {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
