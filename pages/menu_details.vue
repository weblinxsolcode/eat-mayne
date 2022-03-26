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
        <i class="fas fa-bars"
          style="color: #7d2883; font-size: 26px"
        ></i>
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

    <div class="container py-5 mt-5">
      <div class="col-12">
        <div>
          <h1><b>Pressed Cafe Menu</b></h1>
        </div>
        <p class="text-start text-muted col-12 col-lg-4">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
        <!-- <button
            class="btn text-lg-start bg-purple-d-a text-white button-radius-a px-3"
            type="submit"
          >
            Back
          </button> -->
      </div>
    </div>

    <div class="container bg-white rounded-4">
      <div class="row flex-wrap py-5">
        <div class="col-md-4 col-12 col-lg-4 img">
          <img
            src="~assets/images/menu.detail.img.png"
            alt=""
            class="img-fluid my-auto"
          />
        </div>
        <div class="col-md-4 text-start px-4 py-4">
          <h1 class="fs-3 text-start fw-bold"><b>Chocolate Milkshake</b></h1>
          <p class="text-muted">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the industry's standard dummy text
            ever since the 1500s, when an unknown printer took a galley of type
            and scrambled it to make a type specimen book. It has survived not
            only five centuries, but also the leap into electronic typesetting,
            remaining essentially unchanged.
          </p>
          <hr />
          <p class="text-muted" style="font-size: 11px">
            Lorem Ipsum is simply dummy text
          </p>
        </div>
        <div class="col-12 col-md-4 col-lg-4 mt-3">
          <div class="row my-4">
            <div class="col-12 col-md-5 text-center">
              <h6 class="fw-bold text-lg-start ms-0 ms-lg-3">Overall</h6>
              <button class="btn">
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
              </button>
            </div>
            <div class="col-12 col-md-5 text-center mt-4 mt-lg-0">
              <h6 class="fw-bold text-lg-start ms-0 ms-lg-3">Spice</h6>
              <button class="btn">
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
              </button>
            </div>
          </div>
          <!-- row 2 -->
          <div class="row my-4">
            <div class="col-12 col-md-5 text-center">
              <h6 class="fw-bold text-lg-start ms-0 ms-lg-3">Taste</h6>
              <button class="btn">
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </button>
            </div>
            <div class="col-12 col-md-5 text-center mt-4 mt-lg-0">
              <h6 class="fw-bold text-lg-start ms-0 ms-lg-3">Proportion</h6>
              <button class="btn">
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star bg-yellow"></span>
                  <span class="fa fa-star"></span>
                </div>
              </button>
            </div>
          </div>
          <!-- row 3 -->
          <div class="row my-4">
            <div class="col-12 text-center col-md-5">
              <h6 class="fw-bold text-lg-start ms-0 ms-lg-3">Value</h6>
              <button class="btn">
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- center section -->
    <div class="container mt-5">
      <div class="row d-flex flex-wrap">
        <div
          class="col-12 col-md-4 col-lg-4 d-flex justify-content-center flex-column align-items-center"
        >
          <div class="d-flex justify-content-center align-items-center">
            <div class="d-flex justify-content-center align-item-center">
              <p class="four fs-1 fw-bold">4</p>
              <p class="loremp text-muted flex mt-0 mt-lg-2 ms-2 fw-bold">
                Out of<br />5 stars
              </p>
            </div>

            <div class="star mb-2 mb-lg-4 mx-5">
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star bg-yellow"></span>
              <span class="fa fa-star"></span>
            </div>
          </div>
          <div
            class="d-flex justify-content-center align-items-center mt-0 me-0 me-lg-5"
          >
            <p class="text-muted fw-bold me-2" style="font-size: 12px">
              Lorem Ipsum is
            </p>
            <p class="fw-bold" style="font-size: 12px; color: #7d2883">
              ( 454 reviews )
            </p>
          </div>
        </div>

        <div
          class="col-12 col-md-4 col-lg-4 text-center text-lg-start text-muted mt-2"
        >
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </div>

        <div
          class="col-12 col-md-4 col-lg-4 d-flex justify-content-center align-items-start px-0 px-lg-5"
        >
          <button
            class="btn mt-3 bg-purple-d text-white button-radius"
            type="submit"
          >
            Leave us Feedback
          </button>
        </div>
      </div>
    </div>

    <div class="container">
      <VueSlickCarousel class="mx-0 mt-3 mb-4">
        <div class="carousel-item">
          <div class="container">
            <div class="row row2">
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord flex-end px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
              <div class="col-2 d-sm-none"></div>
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="carousel-item">
          <div class="container">
            <div class="row row2">
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord flex-end px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
              <div class="col-2 d-sm-none"></div>
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="carousel-item">
          <div class="container">
            <div class="row row2">
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord flex-end px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
              <div class="col-2 d-sm-none"></div>
              <div
                class="col-12 col-lg-5 col-md-5 bg-white mx-lg-5 mx-0 mx-md-5 cord px-2 py-5 ansab"
              >
                <div class="d-flex xzy">
                  <img
                    src="~assets/images/pexels-anthony-shkraba-7579120.png"
                    class="rounded-circle"
                    width="50px"
                    height="50px"
                    alt=""
                  />
                  <b>
                    <h6 class="py-3 px-3 fs-4">Nancy</h6>
                  </b>
                </div>

                <div class="xzy">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit.
                  Porro, facilis nihil? Iure aspernatur unde autem repellat ab
                  repudiandae quasi cum architecto! Cum, temporibus quisquam sed
                  quo vero impedit voluptas aperiam.
                </div>
                <div class="row">
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                  <div class="col-4 text-center">
                    <b>
                      <h6 class="mt-3 fs-5 d-block">over all</h6>
                    </b>
                    <!-- <button class="btn border border-1 rounded-pill"> -->
                    <div class="star">
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked bg-yellow"></span>
                      <span class="fa fa-star checked"></span>
                      <span class="fa fa-star"></span>
                      <span class="fa fa-star"></span>
                    </div>
                    <!-- </button> -->
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- </div> -->
      </VueSlickCarousel>
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
