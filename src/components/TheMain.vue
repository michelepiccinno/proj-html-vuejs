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
    },
    squareObjects: {
      type: Array,
      required: true,
    },
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
            <h1 class="section-title section-title-left lh-base font-weight-600">We Are Here To &nbsp; Make Your <span
                class="txt-green">Website</span>
              Look More <span class="txt-green">Elegant</span> And
              Stylish!</h1>
            <img class="pb-4 d-block mt-5 mb-4" src="/src/assets/imgs/hr.jpg" alt="">
            <button class="btn button-green text-white">VIEW ALL</button>
          </div>
          <div class="col-7">
            <div class="row g-4">
              <div class="col-6 position-relative" v-for="card in cardObjects">
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
    <section class="third-section">
      <div class="row">
        <div class="col-7">
          <div class="box-img">
            <img src="/src/assets/imgs/busy-architect.jpg" alt="">
            <img class="img-businesswoman" src="/src/assets/imgs/businesswoman.jpg" alt="">
            <div class="ombra"></div>
          </div>
        </div>
        <div class="col-5">
          <div class="box-sect">
            <h1 class="section-title lh-base font-weight-600">
              learn more<br>
              about our<br>
              <span class="txt-green">mission</span>
            </h1>
            <img class="pb-4 d-block mt-4 mb-3" src="/src/assets/imgs/hr.jpg" alt="">
            <p class="text-secondary pb-3">
              Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the
              blind
              texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
              ocean.Separated they live in Bookmarksgrove.
            </p>
            <button class="btn button-green text-white">VIEW ALL</button>
          </div>
        </div>
      </div>
    </section>
    <!-- /SECTION 3 -->

    <!-- SECTION 4 -->
    <section class="fourth-section">
      <div class="container">
        <div class="row row-cols-2">
          <div class="col">
            <img class="pb-4 d-block mt-4 mb-3" src="/src/assets/imgs/hr.jpg" alt="">
            <h1 class="section-title lh-base font-weight-600">
              Our recent <span class="txt-green">web designs</span> &<br>
              some examples of<br>
              past <span class="txt-green">projects</span>
            </h1>
            <img class="pb-4 d-block mt-4 mb-3" src="/src/assets/imgs/hr.jpg" alt="">
          </div>
          <div class="col d-flex align-items-end">
            <p class="pb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet, quaerat blanditiis aliquam
              perspiciatis
              architecto neque molestias recusandae deleniti, temporibus molestiae delectus? Aperiam inventore earum
              facilis. Maiores unde consequatur nihil et!</p>
          </div>
        </div>
        <!-- SQUARE -->
        <div class="row row-cols-4 mt-4 g-1">
          <div class="col" v-for="square in squareObjects">
            <div class="img-box position-relative">
              <img class="img-square mw-100 rounded" :src="square.src" alt="">
              <div class="ombra rounded"></div>
              <div class="text-box text-white">
                <h3>{{ square.title }}</h3>
                <span class="pe-3">{{ square.subTitleOne }}</span>
                <span>{{ square.subTitleTwo }}</span>
              </div>
            </div>
          </div>
          <div class="box-vertical-text">
            <p>17 years of experience helping people for best solutions</p>
          </div>
        </div>

        <!-- /SQUARE -->
        <div class="d-flex justify-content-center m-2">
          <button class="btn button-green text-white z-index200">READ MORE</button>
        </div>
      </div>
    </section>
    <!-- /SECTION 4 -->

    <!-- SECTION 5 -->
    <section class="fifth-section">
      <div class="container">
        <div class="row">
          <div class="col position-relative">
            <div class="box-img">
              <img class="img-pc-woman" src="/src/assets/imgs/person-with-long-curly-hair.jpg" alt="">
              <div class="ombra"></div>
              <div class="text-box text-white text-center">
                <div class="d-flex flex-column">
                  <h1>280</h1>
                  <h2 class="pt-2 pb-5">PROJECTS</h2>
                </div>
                <div class="d-flex gap-5">
                  <div>
                    <h5>+3,500</h5>
                    <h6>USERS' COMMENTS</h6>
                  </div>
                  <div>
                    <h5>+3,500</h5>
                    <h6>USERS' COMMENTS</h6>
                  </div>
                </div>
              </div>
            </div>
            <div class="box-right-text bg-white">
              <h1 class="section-title lh-base font-weight-600">
                We <span class="txt-green">Love What</span>
                <p>We Do</p>
              </h1>
              <img class="pb-4" src="/src/assets/imgs/hr.jpg" alt="">
              <p class="text-secondary pb-4">
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the
                blind
                texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language
                ocean.Separated they live in Bookmarksgrove.
              </p>
              <ul class="list-unstyled">
                <li><span class="txt-green"><i class="fa-solid fa-check"></i></span> &nbsp;far far away, behind the word
                  mountains</li>
                <li class="mt-3 mb-3"><span class="txt-green"><i class="fa-solid fa-check"></i></span> &nbsp;large
                  language ocean</li>
                <li><span class="txt-green"><i class="fa-solid fa-check"></i></span> &nbsp;far from the countries Vokalia
                  and Consonantia</li>
              </ul>
            </div>

          </div>
        </div>
      </div>
    </section>
    <!-- /SECTION 5 -->
  </main>
</template>

<style lang="scss" scoped>
main {
  padding-top: 200px;
  overflow: hidden;

  .first-section {
    background: #f9f9f9;
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
    position: relative;

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

  .third-section {
    background: #f9f9f9;

    .box-img {
      width: 800px;
      border-radius: 0 35px 35px 0;
      position: relative;
      box-shadow: 0 3px 35px 0 rgba(0, 0, 0, .14);

      img {
        width: 100%;
        border-radius: 0 35px 35px 0;
      }

      .ombra {
        width: 100%;
        border-radius: 0 35px 35px 0;
        background-image: linear-gradient(269deg, #17d6aa 0%, #a4e471 100%);
        opacity: .88;
        position: absolute;
        inset: 0;
      }

      .img-businesswoman {
        position: absolute;
        left: 250px;
        top: 100px;
        z-index: 10;
        border-radius: 35px;
        box-shadow: 0 3px 35px 0 rgba(0, 0, 0, .14);
      }
    }

  }

  .fourth-section {
    .text-box {
      opacity: 0;
      position: absolute;
      bottom: 50px;
      left: 40px;
    }

    .ombra {
      position: absolute;
      inset: 0;
      background-image: linear-gradient(269deg, #17d6aa 0%, #a4e471 100%);
      opacity: 0;
      transition: .8s;
    }

    .img-box:hover .ombra {
      opacity: 0.88;
      z-index: 30;
    }

    .img-box:hover .text-box {
      opacity: 0.88;
      transition: .5s;
      transition-delay: .5s;
      z-index: 30;
    }

    .img-box:hover {
      transition: .5s;
      transform: scale(1.1);
      z-index: 30;
    }

    .box-vertical-text {
      position: relative;
      bottom: 450px;
      left: 1545px;
      transform: rotate(-90deg);
      font-size: 15px;
      font-weight: 700;
      color: #393939;
    }
  }

  .fifth-section {
    background-color: #fcfcfc;

    .box-img {
      width: 900px;
      height: 730px;
      border-radius: 0 35px 35px 0;
      position: relative;
      overflow: hidden;

      .text-box {
        position: absolute;
        top: 210px;
        left: 220px;

        h1 {
          font-size: 130px;
          font-weight: 400;
        }

        h2 {
          font-size: 22px;
          font-weight: 600;
          color: rgba(255, 255, 255, .81);
        }

        h5 {
          font-size: 45px;
          font-weight: 400;
        }

        h6 {
          font-size: 22px;
          font-weight: 600;
          padding-top: 10px;
        }
      }

      img {
        height: 100%;
        border-radius: 35px 35px 35px 35px;
      }

      .ombra {
        width: 100%;
        border-radius: 35px 35px 35px 35px;
        background-image: linear-gradient(269deg, #a4e471 0%, #17d6aa 100%);
        opacity: .88;
        position: absolute;
        inset: 0;
      }
    }

    .box-right-text {
      position: absolute;
      left: 800px;
      top: 100px;
      border-radius: 35px 35px 35px 35px;
      padding: 120px 100px 180px;
      box-shadow: 0 3px 35px 0 rgba(0, 0, 0, .14);
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