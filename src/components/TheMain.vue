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
          <h1 class="font-weight-700">Focus</h1>
          <h1 class="pb-4 font-weight-700">on Your <span class="business-txt">Business</span></h1>
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
            <h1 class="section-title-left lh-base font-weight-600">We Are Here To &nbsp; Make Your <span class="txt-green">Website</span>
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
                  <h3 class="section-title-right pt-4 pb-4">{{ card.title }}</h3>
                  <p>{{ card.parag }}</p>
                </div>
              </div>
              <div class="box-vertical-text">
                <p>17 years of experience helping people for best solutions</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- /SECTION 2 -->

    <!-- SECTION 3 -->
    <section class="third section">

    </section>
    <!-- /SECTION 3 -->




  </main>
</template>

<style lang="scss" scoped>
main {
  padding-top: 200px;

  .first-section {
    background: linear-gradient(180deg, rgba(230, 230, 230, 1) 4%, rgba(250, 250, 250, 1) 40%);
    padding-top: 60px;
    padding-bottom: 70px;
    margin-top: -65px;

    .first-section-left {
      margin-left: 100px;
      ;

      .left-text {
        padding-top: 100px;
        padding-left: 70px;

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
    background-color: white;
    padding-top: 114px;
    z-index: 20;
   /* position: relative;*/

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
      right: 12px;
      bottom: 0;
      transition: .8s;
      color: white;
      background-image: linear-gradient(39deg, #00d9a6 0%, #9be15d 100%);
    }

    .card i {
      font-size: 4rem;
      color: #00d9a6;
    }

    .card:hover i {
      transition: .8s;
      color: white;
    }

    .card:hover h3 {
      transition: .8s;
      color: white;
    }

    .card:hover p {
      transition: .8s;
      color: white;
    }

    .box-sect-left {
      padding: 5rem;

      .section-title-left {
        font-size: 55px;
      }


    }

    .box-vertical-text {
      position: relative;
      bottom: 650px;
      left: 550px;
      transform: rotate(-90deg);
      font-size: 15px;
      font-weight: 700;
      color: #393939;
    }
  }


  /*altro css comune*/
  .first-section .img-man {
    border-radius: 50%;
    border: 60px solid lightgrey;
    position: absolute;
    top: -80px;
    left: 165px;
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
    transition: .8s;
  }

  .button-green:hover {
    opacity: .5;
  }

  .txt-green {
    color: #00d9a6;
  }

}
</style>