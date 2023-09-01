<script>
export default {
  props: {
    myString: String,
  }
}
</script>

<template>
  <main class="text-black">
    <section class="first-section">
      <div class="first-section-left d-flex">

        <div class="left-text">
          <h4 class="pb-4">17 YEARS OF EXPERIENCE</h4>
          <h1>Focus</h1>
          <h1 class="pb-4">on Your <span class="business-txt">Business</span></h1>
          <p class="text-secondary">
            Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the
            blind
            texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
            ocean.Separated they live in Bookmarksgrove.
          </p>
        </div>

        <div>
          <img src="/src/assets/imgs/uomo-che-fa-finta-di-pensare.jpg" alt="">
        </div>
      </div>



      <h1>Scrivo tramite PROPS: {{ myString }}</h1>
    </section>
  </main>
</template>

<style lang="scss" scoped>
main {
  position: relative;
  z-index: -10;
  padding-top: 200px;

  .first-section {
    background-color: #fafafa;
  }

  .first-section img {
    border-radius: 50%;
    border: 60px solid lightgrey;
    position: relative;
    top: -90px;
    right: -130px;
  }

  .first-section-left {
    margin-left: 100px;

    .left-text {
      padding-top: 100px;

      h4 {
        color: #00d9a6;
      }

      .business-txt {
        color: #00d9a6;
      }
    }
  }
}</style>