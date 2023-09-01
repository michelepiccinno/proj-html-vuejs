<script>
export default {
  props: {
    navTextElement: {
      type: Array,
      required: true,
    }
  }
}

</script>

<template>
  <div class="header-container vw-100 position-fixed">
    <!-- HEADER TOP -->
    <div class="header-box">
      <div class="container-fluid">
        <div class="row text-white align-items-center">
          <div class="col d-flex justify-content-between">
            <div>
              <i class="fa-solid fa-phone"></i>
              <span>&nbsp; (001) 88451234&nbsp; &nbsp; &nbsp;88455438</span>
            </div>
            <div class="d-flex align-items-center gap-4">
              <i class="fa-brands fa-facebook-f"></i>
              <i class="fa-brands fa-twitter"></i>
              <i class="fa-brands fa-pinterest-p"></i>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- /HEADER TOP -->

    <!-- HEADER NAV -->
    <div class="header-box bg-white pt-4 pb-4">
      <div class="container-fluid">
        <div class="row">
          <div class="col-3">
            <img src="/src/assets/imgs/logo-header.png" alt="">
          </div>
          <div class="col-6 d-flex align-items-end">

            <ul class="d-flex justify-content-between list-unstyled w-100 text-uppercase">
              <li class="nav-item" v-for="element in navTextElement">
                <a class="nav-link" href="#">{{ element }}</a>
              </li>
            </ul>

          </div>
          <div class="col-3 d-flex justify-content-end">
            <button class="btn btn-warning text-white">PURCHASE</button>
            <i class="fa-solid fa-magnifying-glass"></i>
          </div>
        </div>
      </div>
    </div>
    <!-- /HEADER NAV -->
  </div>
</template>


<style lang="scss" scoped>
.header-box {
  background-color: #3b3b3b;
  padding: .7rem 5rem .7rem 5rem;

  .fa-phone {
    line-height: unset;
  }

  button {
    padding: 0 45px 0 45px;
    background-color: transparent;
    --bs-border-radius: 2rem;
    border: none;
    background-image: linear-gradient(269deg, #00d9a6 0%, #9be15d 100%);
    box-shadow: 6px 6px 25px 0 rgba(0, 217, 166, .35);
    text-shadow: 0 0 10px rgba(0, 0, 0, .04);
    font-size: .9rem;
  }

  button :hover {
    opacity: .5;
  }

  .fa-magnifying-glass {
    line-height: 55px;
    padding-left: 20px;
    color: #00d9a6;
  }

  li :hover {
    font-weight: 500;
  }
}
</style>

