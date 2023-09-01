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
          <h4 class="pb-4">1 7 &nbsp;Y E A R S &nbsp;O F &nbsp;E X P E R I E N C E</h4>
            <h1>Focus</h1>
            <h1 class="pb-4">on Your <span class="business-txt">Business</span></h1>
          <p class="text-secondary pb-4">
            Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the
            blind
            texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
            ocean.Separated they live in Bookmarksgrove.
          </p>
          <button class="btn btn-dark">READ MORE</button>
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

      h1 {
        font-size: 5rem;
      }

      h4 {
        font-size: 1.1rem;
        color: #00d9a6;
      }

      .business-txt {
        color: #00d9a6;
      }

      .btn-dark {
        border-radius: 50px;
        font-size: .8rem;
        padding: 1rem 3rem;
      }
    }
  }
}
</style>