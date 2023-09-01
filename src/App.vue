<script>
import TheHeader from "./components/TheHeader.vue";
import TheTheMain from "./components/TheMain.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheTheMain,
    TheFooter
  },
  data() {
    return {
    };
  },
};
</script>

<template>
  <TheHeader></TheHeader>
  <TheTheMain :myString="`main by props`"></TheTheMain>
  <TheFooter></TheFooter>
</template>

<style lang="scss">
template {
  font-family: Sans-serif,Arial, Helvetica;
}
</style>











