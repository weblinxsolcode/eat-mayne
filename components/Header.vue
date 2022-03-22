<template>
  <div>
    <!-- nav bar -->
    <b-navbar
      toggleable="lg"
      type="transparent"
      class="container mt-3"
      variant="transparent"
    >
      <span v-b-toggle.sidebar-backdrop>
        <i
          class="fas fa-angle-double-down"
          style="color: #7d2883; font-size: 26px"
        ></i>
      </span>
      <b-navbar-brand href="#">
        <NuxtLink to="/">
          <img class="ms-5" height="30px" src="~assets/images/logo.png" alt=""/>
        </NuxtLink>
      </b-navbar-brand>

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

    <!-- offset -->
    <div>
      <b-sidebar
        width="400px"
        id="sidebar-backdrop"
        title="Sidebar with backdrop"
        :backdrop-variant="variant"
        backdrop
        shadow
      >
        <div class="p-5">
          <div class="d-flex flex-column">
            <p class="text-muted mb-1" style="font-size: 12px">
              Restaurant Name
            </p>
            <h2 class="my-0 py-0 fw-bold text-start">Pressed Cafe</h2>
          </div>
          <div class="my-5">
            <h5 class="text-purple-d fw-bold">Address</h5>
            <p class="mb-0 mt-3 text-muted">
              Lorem ipsum dolor sit amet consectetur adipi
            </p>
          </div>
          <div class="my-5">
            <h5 class="text-purple-d fw-25 fw-bold">Hours</h5>
            <p class="mb-0 mt-3 text-muted">Lorem ipsum dolor</p>
          </div>
          <div class="my-5">
            <h5 class="text-purple-d fw-bold">Rating</h5>
            <div class="star_1">
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star checked bg-yellow"></span>
              <span class="fa fa-star bg-yellow"></span>
              <span class="fa fa-star"></span>
              <span style="color: gray; font-size: small">(454 reviews)</span>
            </div>
          </div>
          <div class="mt-4">
            <h5 class="text-purple-d fw-bold">Calls</h5>
            <p class="mb-0 mt-3 text-muted">Lorem ipsum dolor sit</p>
          </div>
          <div class="mt-5">
            <button
              class="btn mx-4 text-lg-center bg-purple-d-a text-white button-radius-a"
            >
              Rate this Restaurant
            </button>
          </div>
        </div>
      </b-sidebar>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      variant: "dark",
      variants: [
        "transparent",
        "white",
        "light",
        "dark",
        "primary",
        "secondary",
        "success",
        "danger",
        "warning",
        "info",
      ],
    };
  },
};
</script>
