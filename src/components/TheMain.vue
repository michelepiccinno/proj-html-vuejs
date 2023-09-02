<script>
export default {
  props: {
    socialTextElement: {
      type: Array,
      required: true,
    },
    cardObjects: {
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
          <button class="section1-button btn btn-dark">READ MORE</button>
          <ul class="social-link-box d-flex gap-4 list-unstyled">
            <li class="social-item" v-for="element in socialTextElement">
              <a class="nav-link" href="#">{{ element }}</a>
            </li>
          </ul>
        </div>
        <div class="position-relative">
          <img class="img-man" src="/src/assets/imgs/uomo-che-fa-finta-di-pensare.jpg" alt="">
        </div>
      </div>
    </section>
    <!-- /SECTION 1 -->

    <!-- SECTION 2 -->
    <section class="second-section">
      <div class="container">
        <div class="row">
          <div class="box-sect-left col-5">
            <h1 class="section-title-left lh-base">We Are Here To &nbsp; Make Your <span class="txt-green">Website</span>
              Look More <span class="txt-green">Elegant</span> And
              Stylish!</h1>
            <img class="pb-4 d-block mt-5 mb-4" src="/src/assets/imgs/hr.jpg" alt="">
            <button class="btn button-green text-white">VIEW ALL</button>
          </div>
          <div class="col-7">
            <div class="row g-4">
              <div class="col-6 position-relative" v-for="(card) in cardObjects">
                <div class="card">
                  <i :class="card.icon"></i>
                  <h3 class="section-title-right">{{ card.title }}</h3>
                  <p>{{ card.parag }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- /SECTION 2 -->

  </main>
</template>

<style lang="scss" scoped>
main {
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
          position: absolute;
        }

        .social-link-box {
          margin-top: 180px;
          font-weight: 500;

          .nav-link:hover {
            background: -webkit-linear-gradient(45deg, #00d9a6, #9be15d);
            -webkit-text-fill-color: transparent;
            -webkit-background-clip: text;
            color: transparent;
          }
        }

        .section1-button:hover {
          background: #00d9a6;
          border: none;
          transform: scale(.99);
          box-shadow: 6px 6px 25px 0px rgba(0, 0, 0, 0.35);
          transition: .5s;
        }
      }
    }
  }

  .second-section {
    margin-top: 200px;

    .card {
      padding: 3rem;
      border: none;
      border-radius: 15px;
      box-shadow: 0 3px 35px 0 rgba(0, 0, 0, .14);
    }

    .card>p {
      color: grey;
    }

    .card:hover {
      position: absolute;
      left: 12px;
      top: 0;
      right: 0;
      bottom: 0;
      transition: .4s;
      color: white;
      background-image: linear-gradient(39deg, #00d9a6 0%, #9be15d 100%);
    }

    .card i {
      font-size: 4rem;
      color: #00d9a6;
    }

    .card:hover i {
      transition: .4s;
      color: white;
    }

    .card:hover p {
      transition: .4s;
      color: white;
    }

    .box-sect-left {
      padding: 5rem;

      .section-title-left {
        font-size: 3.5rem;
        font-weight: 600;
      }
    }
  }




  /*altro css comune*/
  .first-section .img-man {
    border-radius: 50%;
    border: 60px solid lightgrey;
    position: absolute;
    top: -80px;
    left: 240px;
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

  .txt-green {
    color: #00d9a6;
  }

}
</style>