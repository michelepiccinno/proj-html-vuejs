<script>
import TheHeader from "./components/TheHeader.vue";
import TheMain from "./components/TheMain.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheMain,
    TheFooter,
  },
  data() {
    return {
      navTextElement: [
        'Home',
        'About',
        'Services',
        'Showcase',
        'Blog',
        'Contact'
      ],
      socialTextElement: [
        'Facebook',
        'Instagram',
        'Twitter',
        'Youtube'
      ],
      cardObjects: [
        {
          icon: 'fa-solid fa-gauge-high',
          title: 'Speed Optimization',
          parag: 'Far far away, behind the word mountains, far from the countries Vokalia Separated...'
        },
        {
          icon: 'fa-solid fa-cloud',
          title: 'Cloud Solutions',
          parag: 'Far far away, behind the word mountains, far from the countries Vokalia Separated...'
        },
        {
          icon: 'fa-solid fa-tablet-screen-button',
          title: 'Website Design',
          parag: 'Far far away, behind the word mountains, far from the countries Vokalia Separated...'
        },
        {
          icon: 'fa-solid fa-stopwatch',
          title: 'Online Marketing',
          parag: 'Far far away, behind the word mountains, far from the countries Vokalia Separated...'
        },

      ],
    }
  }

};
</script>

<template>
  <TheHeader :navTextElement='navTextElement'></TheHeader>
  <TheMain :socialTextElement='socialTextElement' :cardObjects="cardObjects"></TheMain>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
* {
  font-family: 'Quicksand', sans-serif;
}



@media (min-width: 1400px) {
  .container {
    min-width: 1720px;
  }
}
</style>











