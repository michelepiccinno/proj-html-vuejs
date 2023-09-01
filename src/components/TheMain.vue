<script>
export default {
  props: {
    socialTextElement: {
      type: Array,
      required: true,
    }
  }
}
</script>


<template>
  <main class="text-black">
    <!-- SECTION 1 -->
    <section class="first-section">
      <div class="first-section-left d-flex">
        <div class="left-text">
          <h4 class="pb-4">1 7 &nbsp;Y E A R S &nbsp;O F &nbsp;E X P E R I E N C E</h4>
          <h1>Focus</h1>
          <h1 class="pb-4">on Your <span class="business-txt">Business</span></h1>
          <img class="pb-4" src="/src/assets/imgs/hr.jpg" alt="">
          <div class="p-box">
            <p class="text-secondary pb-4">
              Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the
              blind
              texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
              ocean.Separated they live in Bookmarksgrove.
            </p>
          </div>
          <button class="btn btn-dark">READ MORE</button>
          <ul class="social-link-box d-flex gap-4 list-unstyled">
            <li class="social-item" v-for="element in socialTextElement">
              <a class="nav-link" href="#">{{ element }}</a>
            </li>
          </ul>
        </div>
        <div>
          <img class="img-man" src="/src/assets/imgs/uomo-che-fa-finta-di-pensare.jpg" alt="">
        </div>
      </div>
    </section>
    <!-- /SECTION 1 -->

    <!-- SECTION 2 -->
    <section class="second-section">
      <div class="container">
        <div class="row">

          <div class="col-5">
            <h1 class="section-title">We Are Here To
              Make YourWebsite
              Look MoreElegantAnd Stylish!</h1>
            <img class="pb-4 d-block" src="/src/assets/imgs/hr.jpg" alt="">
            <button class="btn button-green text-white">VIEW ALL</button>
          </div>

          <div class="col-7">
            <div class="row">
              <div class="card-box col-6 border">
                <i class="fa-solid fa-gauge-high"></i>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo in obcaecati modi aliquid. Omnis quo
              </div>
              <div class="card-box col-6 border">
                <i class="fa-solid fa-cloud"></i>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo in obcaecati modi aliquid. Omnis quo
              </div>
              <div class="row">
                <div class="card-box col-6 border">
                  <i class="fa-solid fa-tablet-screen-button"></i>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo in obcaecati modi aliquid. Omnis quo
                </div>
                <div class="card-box col-6 border">
                  <i class="fa-solid fa-stopwatch"></i>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo in obcaecati modi aliquid. Omnis quo
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
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

        .p-box {
          max-width: 650px;
        }

        .business-txt {
          color: #00d9a6;
        }

        .btn-dark {
          border-radius: 50px;
          font-size: .8rem;
          padding: 1rem 3rem;
        }

        .social-link-box {
          margin-top: 180px;
          font-weight: 500;
        }


      }
    }
  }

  .second-section {
    .card-box {
      padding: 3rem;
    }

    .card-box:hover {
      background-color: red;
    }

    .section-title {
      font-size: 3.5rem;
      font-weight: 400;
    }
  }




  /*altro css comune*/
  .first-section .img-man {
    border-radius: 50%;
    border: 60px solid lightgrey;
    position: relative;
    top: -90px;
    right: -130px;
  }

  .button-green {
    padding: 15px 45px 15px 45px;
    background-color: transparent;
    --bs-border-radius: 2rem;
    border: none;
    background-image: linear-gradient(269deg, #00d9a6 0%, #9be15d 100%);
    box-shadow: 6px 6px 25px 0 rgba(0, 217, 166, .35);
    text-shadow: 0 0 10px rgba(0, 0, 0, .04);
    font-size: .9rem;
  }





}
</style>