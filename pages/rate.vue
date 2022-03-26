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
      <div class="col-12 w mt-5">
        <div>
          <h1><b>Rate This Restaurant</b></h1>
          <p class="text-muted">
            Lorem Ipsum is simply dummy text of the printing<br />and
            typesetting industry.
          </p>
        </div>
      </div>
      <div class="container bg-white py-2 izan ansab">
        <div class="">
          <div class="container px-0 px-lg-5 my-5">
            <div class="row d-flex flex-wrap">
              <div class="col-12 col-lg-2 my-0 my-lg-4">
                <b
                  ><label class="form-label" for="restaurantName"
                    >Restaurant Name</label
                  ></b
                >
              </div>
              <div class="col-12 col-lg-10">
                <input
                  class="form-control bg-semi-white"
                  id="restaurantName"
                  type="text"
                  placeholder="Type & Search"
                  data-sb-validations=""
                />
              </div>
            </div>

            <div class="row">
              <div class="col-12 col-lg-2 my-0 my-lg-4 mt-4 mt-lg-0">
                <b
                  ><label class="form-label" for="restaurantName"
                    >Dish Name</label
                  ></b
                >
              </div>
              <div class="col-12 col-lg-10">
                <input
                  class="form-control bg-semi-white"
                  id="restaurantName"
                  type="text"
                  placeholder="Prepopulated"
                  data-sb-validations=""
                />
              </div>
            </div>

            <div class="row">
              <div class="col-12 col-lg-2"></div>
              <div class="col-12 col-lg-10 d-flex flex-wrap">
                <div class="col-12 col-lg-6">
                  <label class="form-label" for=""></label>
                  <input
                    class="form-control bg-semi-white"
                    id=""
                    type="text"
                    placeholder="Spice"
                    data-sb-validations=""
                  />
                </div>
                <div class="col-12 col-lg-6">
                  <label class="form-label" for=""></label>
                  <input
                    class="form-control bg-semi-white mx-0"
                    id=""
                    type="text"
                    placeholder="Portion"
                    data-sb-validations=""
                  />
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col-12 col-lg-2"></div>
              <div class="col-12 col-lg-10 d-flex flex-wrap">
                <div class="col-12 col-lg-6">
                  <label class="form-label" for=""></label>
                  <input
                    class="form-control bg-semi-white"
                    id=""
                    type="text"
                    placeholder="Value"
                    data-sb-validations=""
                  />
                </div>
                <div class="col-12 col-lg-6">
                  <label class="form-label" for=""></label>
                  <input
                    class="form-control bg-semi-white mx-0"
                    id=""
                    type="text"
                    placeholder="Mayne Factor"
                    data-sb-validations=""
                  />
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col-12 col-lg-2"></div>
              <div class="col-12 col-lg-10">
                <label class="form-label" for=""></label>
                <input
                  class="form-control bg-semi-white"
                  id=""
                  type="text"
                  placeholder="Overall"
                  data-sb-validations=""
                />
              </div>
            </div>

            <div class="row">
              <div class="col-12 col-lg-2">
                <b>
                  <label class="form-label mt-2" for="comments"
                    >Comments</label
                  ></b
                >
              </div>
              <div class="col-12 col-lg-10">
                <textarea
                  class="form-control bg-semi-white my-3"
                  id="comments"
                  type="text"
                  placeholder="Description"
                  style="height: 10rem"
                  data-sb-validations=""
                ></textarea>
              </div>
            </div>

            <hr class="my-5" />
            <div class="col-12 text-center">
              <div class="rating-css">
                <div class="star-icon">
                  <input type="radio" name="rating1" id="rating1" />
                  <label for="rating1" class="fa fa-star"></label>
                  <input type="radio" name="rating1" id="rating2" />
                  <label for="rating2" class="fa fa-star"></label>
                  <input type="radio" name="rating1" id="rating3" />
                  <label for="rating3" class="fa fa-star"></label>
                  <input type="radio" name="rating1" id="rating4" />
                  <label for="rating4" class="fa fa-star"></label>
                  <input type="radio" name="rating1" id="rating5" />
                  <label for="rating5" class="fa fa-star"></label>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
