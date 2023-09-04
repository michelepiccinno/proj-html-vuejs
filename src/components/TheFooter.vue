<script>
export default {
  props: {
    footerMenuElements: {
      type: Array,
      required: true,
    },
  },
}
</script>

<template>
  <!-- FOOTER -->
  <section>
    <div class="container">
      <div class="row row-cols-4">
        <div class="col">
          <img class="mb-3" src="/src/assets/imgs/logo-header.png" alt="">
          <p>While the lovely valley teems with vapour around me, and the meridian sun strikes the upper surface of the
            impenetrable foliage of my trees.While the lovely valley teems with vapour around me.</p>
        </div>
        <div class="col">
          <h6 class="menu-title">QUICk LINKS</h6>
          <ul class="list-unstyled">
            <img class="img-hr" src="/src/assets/imgs/hr.jpg" alt="">
            <li v-for="element in footerMenuElements" class="mb-1">{{ element }}</li>
          </ul>
        </div>
        <div class="col">
          <h6 class="menu-title">CONTACT</h6>
          <img class="img-hr" src="/src/assets/imgs/hr.jpg" alt="">
          <div>
            <p class="mb-3">Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, TX 76051</p>
            <p class="mb-3">info@yourdomain.com</p>
            <p class="mb-3">+99 (0) 101 0000 888</p>
          </div>
        </div>
        <div class="col">
          <h6 class="menu-title">LOCATION ON MAP</h6>
          <img class="img-hr" src="/src/assets/imgs/hr.jpg" alt="">
          <div style="width: 100%">
            <iframe width="100%" height="200" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"
              src="https://maps.google.com/maps?width=100%25&amp;height=200&amp;hl=en&amp;q=1%20Grafton%20Street,%20Dublin,%20Ireland+(My%20Business%20Name)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed">
            </iframe>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div class="footer-bottom-container d-flex justify-content-between">
    <span class="footer-bottom-text">© 2023 PHLOX BUSINESS THEME.</span>
    <div class="d-flex align-items-center gap-4">
      <i class="fa-brands fa-facebook-f"></i>
      <i class="fa-brands fa-twitter"></i>
      <i class="fa-brands fa-pinterest-p"></i>
    </div>
  </div>

  <!-- /FOOTER -->
</template>

<style lang="scss" scoped>

.img-hr {
  margin: 20px 0;
}

.menu-title {
  color: #444;
  font-size: 23px;
  font-weight: 700;
}

.footer-bottom-container {
  background-color: #313131;
  padding: 35px 100px;

  .footer-bottom-text {
    color: #ffffff80;
    font-size: small;
  }

  .fa-brands {
    color: #898989;
  }
}
</style>