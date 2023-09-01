<script>
import TheHeader from "./components/TheHeader.vue";
import TheTheMain from "./components/TheMain.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheTheMain,
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
      ]
    }
  }

};
</script>

<template>
  <TheHeader :navTextElement='navTextElement'></TheHeader>
  <TheTheMain :socialTextElement='socialTextElement'></TheTheMain>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
template {
  font-family: Sans-serif, Arial, Helvetica;
}

@media (min-width: 1400px) {
.container {
    min-width: 1720px;
}
}
</style>











