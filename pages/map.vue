<template>
  <div>
    <!-- nav bar -->
    <b-navbar
      toggleable="lg"
      type="transparent"
      class="container mt-3"
      variant="transparent"
    >
      <!-- <span v-b-toggle.sidebar-backdrop>
        <i class="fas fa-bars" style="color: #7d2883; font-size: 26px"></i>
      </span> -->
      <!-- <b-navbar-brand href="#"> -->
      <NuxtLink to="/">
        <img class="ms-5" height="30px" src="~assets/images/logo.png" alt="" />
      </NuxtLink>
      <!-- </b-navbar-brand> -->

      <b-navbar-toggle target="nav-collapse">
        <i class="fas fa-bars" style="color: black"></i>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ms-auto mt-2">
          <b-nav-item class="mx-2 fw-bold">
            <NuxtLink to="/rate"> Rate Now </NuxtLink>
          </b-nav-item>
          <b-nav-item class="mx-2 fw-bold">
            <NuxtLink to="/map"> View Map </NuxtLink>
          </b-nav-item>
          <b-nav-form class="">
            <b-input-group>
              <b-input-group-text
                class="py-3 mt-0"
                style="border: none; background-color: #f7f4f7"
              >
                <i class="fas fa-search text-muted"></i>
              </b-input-group-text>
              <b-form-input
                class="mt-0 pt-1"
                placeholder="Find Dish Name..."
                style="border: none; background-color: #f7f4f7"
              ></b-form-input>
            </b-input-group>
          </b-nav-form>
        </b-navbar-nav>

        <b-navbar-nav class="ms-auto">
          <button
            href="#"
            class="btn text-decoration-underline mx-3 border-0 bg-white fw-bold"
          >
            Sign In
          </button>
          <button
            class="btn bg-purple-d text-white button-radius px-3 fw-bold"
            type="submit"
          >
            Sign-Up
          </button>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <div class="container py-5">
      <div class="">
        <div>
          <b> <h1>Search</h1></b>
        </div>
        <div class="">
          <input
            type="text"
            class="mt-3 form-control border-3 width1 w-100"
            placeholder="Search Now ..."
            aria-label="Username"
            aria-describedby="basic-addon1"
          />
        </div>
        <div class="flex-column mt-5 ms-0">
          <iframe
            class="w-100"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14474.478712135166!2d67.2007256!3d24.9109513!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3eb3377b02c89ec7%3A0x8f7391d696dcb02e!2sMalir%20Cantt%20Check%20Post%20No%202%2C%20Malir%20Cantonment%2C%20Karachi%2C%20Karachi%20City%2C%20Sindh%2C%20Pakistan!5e0!3m2!1sen!2s!4v1647017407180!5m2!1sen!2s"
            width="600"
            height="450"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
          ></iframe>
        </div>
      </div>

      <!-- CARDS -->
      <div class="container">
        <VueSlickCarousel class="mx-0 mt-3 mb-4">
          <!-- Card 1 -->
          <div class="d-flex justify-content-between">
            <div class="va-card d-flex flex-row align-items-center">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>

            <div class="va-card d-flex flex-row align-items-center for_hide">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>
          </div>

          <div class="d-flex justify-content-between">
            <div class="va-card d-flex flex-row align-items-center">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>

            <div class="va-card d-flex flex-row align-items-center for_hide">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>
          </div>

          <div class="d-flex justify-content-between">
            <div class="va-card d-flex flex-row align-items-center">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>

            <div class="va-card d-flex flex-row align-items-center for_hide">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>
          </div>

          <div class="d-flex justify-content-between">
            <div class="va-card d-flex flex-row align-items-center">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>

            <div class="va-card d-flex flex-row align-items-center for_hide">
              <div>
                <img class="va-thumbnail" src="~assets/images/222.png" />
              </div>
              <div class="d-flex flex-column align-items-start px-3 flex-wrap">
                <div class="va-title text-muted">Pressed Cafe</div>
                <div class="va-start-from">
                  105 Humilton Ave, Boston,NY
                  <span style="color: rgb(238, 100, 58)"> 17m </span>
                </div>
                <div class="star text-start w-100">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </div>
            </div>
          </div>
        </VueSlickCarousel>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
export default {
  name: "MyComponent",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        arrows: true,
        dots: false,
        slidesToShow: 2,
      },
    };
  },
};
</script>
