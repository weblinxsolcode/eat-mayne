<template>
  <div>
    <!-- nav bar -->
    <b-navbar
      toggleable="lg"
      type="transparent"
      class="container mt-3"
      variant="transparent"
    >
      
      <NuxtLink to="/">
        <img class="ms-5" height="30px" src="~assets/images/logo.png" alt="" />
      </NuxtLink>

      <b-navbar-toggle target="nav-collapse">
        <i class="fas fa-bars" style="color: black"></i>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ms-auto mt-2 text-center">
          <b-nav-form>
            <b-input-group class="search_feild">
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
          <b-nav-item class="mx-2 fw-bold">
            <NuxtLink to="/rate"> Rate Now </NuxtLink>
          </b-nav-item>
          <b-nav-item class="mx-2 fw-bold">
            <NuxtLink to="/map"> View Map </NuxtLink>
          </b-nav-item>
          <!-- </b-navbar-nav> -->

          <!-- <b-navbar-nav class="ms-auto"> -->
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

    <!-- section banner start -->
    <section class="banner pt-2 mt-5">
      <div class="container">
        <div class="container">
          <div class="row d-flex flex-wrap align-items-center">
            <div class="col-md-6 text-lg-start text-center pt-1">
              <b>
                <h1 class="h1-a mx-4">Lorem Ipsum is</h1>
              </b>
              <b>
                <h1 class="h1-a mx-4">simply dummy text</h1>
              </b>
              <p class="text-secondary mx-4">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry.
              </p>
              <NuxtLink to="/menu">
                <button
                  class="btn mx-4 text-lg-center bg-purple-d-a text-white button-radius-a"
                >
                  Lorem Ipsum
                </button>
              </NuxtLink>
            </div>
            <!-- banner img -->
            <div
              class="brain col-md-6 justify-content-center align-item-center mt-5 mt-lg-0 mt-md-0"
            >
              <img
                src="~assets/images/bannner.png"
                class="img-fluid my-auto"
                alt=""
              />
              <div class="reviews_rate">
                <p class="fw-bold">
                  4.5 <span class="text-muted">( 1000+ review )</span>
                </p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <div class="chars">
                  <img class="char1" src="~assets/images/char1.png" alt="" />
                  <img src="~assets/images/char2.png" alt="" />
                  <img src="~assets/images/char3.png" alt="" />
                  <img src="~assets/images/char4.png" alt="" />
                </div>
              </div>
              <div class="ban_lorem">
                <p class="fw-bold">Lorem Ipsum dumy text</p>
                <p class="text-muted">Lorem Ipsum is simply dummy text</p>
              </div>
              <!-- <img clas src="~assets/images/Rectangle 1.png" alt="" /> -->
              <!-- <img src="~assets/images/Rectangle 2.png" alt="" /> -->
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- section banner end -->
    <!-- card 1 -->
    <section class="center-id mb-5">
      <div class="container py-5">
        <div class="row d-flex">
          <div
            class="col-12 col-md-2 col-lg-2 radius bg-white card-1 pt-3 mx-auto"
            id="radio1"
          >
            <label class="container123 text-muted fw-bold">
              Thai
              <input type="checkbox" class="na" checked />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Chinese
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Indian
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Amercian
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
          </div>
          <!-- card 2 -->
          <div
            class="card-2 col-12 col-md-5 col-lg-5 m-auto radius my-lg-0 my-md-0 my-3 bg-white justify-content-center align-items-center"
          >
            <div class="d-flex mt-5 justify-content-between align-items-start">
              <!-- <NuxtLink to="/menu_details"> -->
              <button
                class="btn text-lg-start bg-purple-d-a text-white button-radius-a"
                @click="showRadio1"
              >
                Cuisines
              </button>
              <!-- </NuxtLink> -->
              <p class="mx-3 mb-0 ud">Trending Restaurants</p>
            </div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex justify-content-between">
                <p class="text-muted fw-bold fs-5">Pressed Cafe</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  105 Humlington Ave, Boston, NY
                </p>
                <span class="mx-3 bg-pink">1.7m</span>
              </div>
            </div>
            <hr class="hr" />
            <!-- num 2 -->
            <div class="d-flex"></div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Pressed Cafe</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  105 Humlington Ave, Boston, NY
                </p>
                <span class="mx-3 bg-pink">1.7m</span>
              </div>
            </div>
            <hr class="hr" />
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Pressed Cafe</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  105 Humlington Ave, Boston, NY
                </p>
                <span class="mx-3 bg-pink">1.7m</span>
              </div>
            </div>
            <hr class="hr" />
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Pressed Cafe</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  105 Humlington Ave, Boston, NY
                </p>
                <span class="mx-3 bg-pink">1.7m</span>
              </div>
            </div>
            <hr class="hr" />
          </div>
          <!-- card 3 -->
          <div
            class="card-2 col-12 col-md-5 col-lg-5 m-auto radius bg-white justify-content-center align-items-center mt-md-5 mt-lg-0"
          >
            <div class="d-flex justify-content-between mt-5 align-items-start">
              <p class="mb-0 ty ud2">Trending Dishes</p>
              <!-- <NuxtLink to="/menu"> -->
              <button
                class="btn text-end bg-purple-d-a text-white button-radius-a"
                @click="showRadio2"
              >
                Dishes
              </button>
              <!-- </NuxtLink> -->
            </div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Buffalo Wings</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  Pressed Cafe
                </p>
              </div>
            </div>
            <hr class="hr" />
            <div class="d-flex"></div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Buffalo Wings</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  Pressed Cafe
                </p>
              </div>
            </div>
            <hr class="hr" />
            <div class="d-flex"></div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Buffalo Wings</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  Pressed Cafe
                </p>
              </div>
            </div>
            <hr class="hr" />
            <div class="d-flex"></div>
            <div class="padding">
              <div class="col-12 pt-5 d-flex">
                <p class="text-muted fw-bold fs-5">Buffalo Wings</p>
                <div class="star">
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star checked bg-yellow"></span>
                  <span class="fa fa-star"></span>
                  <span class="fa fa-star"></span>
                </div>
                <br />
              </div>
              <div class="col-12 d-flex">
                <p class="text-start fw-bold" style="color: #7d2883">
                  Pressed Cafe
                </p>
              </div>
            </div>
            <hr class="hr" />
          </div>
          <div
            class="col-12 col-md-2 col-lg-2 radius bg-white card-1 pt-3 pb-3 mt-4 mt-lg-0 mx-auto"
            id="radio2"
          >
            <label class="container123 text-muted fw-bold">
              Thai
              <input type="checkbox" class="na" checked />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Chinese
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Indian
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
            <label class="container123 text-muted fw-bold">
              Amercian
              <input type="checkbox" />
              <span class="checkmark"></span>
            </label>
          </div>
        </div>
      </div>
      <!-- </div> -->
    </section>
  </div>
</template>

<script>
export default {
  methods: {
    head() {
      return {
        script: [
          {
            src: "/assets/js/index.js",
          },
        ],
      };
    },
    showRadio1() {
      if (
        document.getElementById("radio2").style.display === "block" &&
        document.getElementById("radio1").style.display === "none"
      ) {
        document.getElementById("radio2").style.display = "none";
        document.getElementById("radio1").style.display = "block";
      } else if (
        document.getElementById("radio2").style.display === "block" ||
        document.getElementById("radio1").style.display === "none"
      ) {
        document.getElementById("radio2").style.display = "none";
        document.getElementById("radio1").style.display = "block";
      } else {
        document.getElementById("radio1").style.display = "none";
      }
    },
    showRadio2() {
      if (
        document.getElementById("radio1").style.display === "block" &&
        document.getElementById("radio2").style.display === "none"
      ) {
        document.getElementById("radio1").style.display = "none";
        document.getElementById("radio2").style.display = "block";
      } else if (
        document.getElementById("radio1").style.display === "block" ||
        document.getElementById("radio2").style.display === "none"
      ) {
        document.getElementById("radio1").style.display = "none";
        document.getElementById("radio2").style.display = "block";
      } else {
        document.getElementById("radio2").style.display = "none";
      }
    },
  },
};
</script>
