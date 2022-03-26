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
        <i class="fas fa-bars" style="color: #7d2883; font-size: 26px"></i>
      </span>
      <!-- <b-navbar-brand href="#"> -->
      <NuxtLink to="/">
        <img class="ms-5" height="30px" src="~assets/images/logo.png" alt="" />
      </NuxtLink>
      <!-- </b-navbar-brand> -->

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
            <NuxtLink to="/rate">
              <button
                class="btn mx-4 text-lg-center bg-purple-d-a text-white button-radius-a"
              >
                Rate this Restaurant
              </button>
            </NuxtLink>
          </div>
        </div>
      </b-sidebar>
    </div>

    <div class="container pt-5 my-5">
      <div class="col-12">
        <div>
          <h1 class="heading_one fw-bold">Pressed Cafe Menu</h1>
        </div>
        <p class="text-start col-lg-5 col-12 text-muted fw-bold">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>

        <!-- <button
          class="btn text-lg-start bg-purple-d-a text-white button-radius-a my-4"
          type="submit"
        >
          Back
        </button> -->
      </div>
    </div>

    <div class="container cord flex-end pt-5">
      <div class="row d-flex flex-wrap">
        <div class="col-12 col-lg-9 uddin bg-white cord flex-end py-4 ansab">
          <!-- <div class="for_shadow"> -->
          <div class="">
            <div class="warpper">
              <input class="radio" id="one" name="group" type="radio" />
              <input class="radio" id="two" name="group" type="radio" />
              <input class="radio" id="three" name="group" type="radio" />

              <div class="aliyan">
                <div
                  class="menu_head text-lg-start text-md-start text-center ps-5 ps-lg-4"
                >
                  <h3 class="menu-h">Most Favorites Items</h3>
                  <p class="text-muted" style="font-size: 13px">
                    Lorem Ipsum is simply dummy text
                  </p>
                </div>
                <div
                  class="tabs mx-3 mx-lg-5 mt-4 mt-lg-0 mt-md-0"
                  style="border-bottom: 1px solid lightgrey"
                >
                  <label class="tab fw-bold text-muted" id="one-tab" for="one"
                    >All Categories</label
                  >

                  <label class="tab fw-bold text-muted" id="two-tab" for="two"
                    >Main Course</label
                  >
                  <label
                    class="tab fw-bold text-muted"
                    id="three-tab"
                    for="three"
                    >Drink</label
                  >
                  <label
                    class="tab fw-bold text-muted"
                    id="three-tab"
                    for="three"
                    >Appetizers</label
                  >
                </div>
              </div>

              <div class="panels">
                <div class="panel" id="one-panel">
                  <div class="panel-title">
                    <div class="row">
                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/roll.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>

                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/orange_juice.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>
                    </div>
                  </div>
                  <p></p>
                </div>

                <div class="panel" id="two-panel">
                  <div class="panel-title">
                    <div class="row">
                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/roll.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>

                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/orange_juice.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>
                    </div>
                  </div>
                  <p></p>
                </div>

                <div class="panel" id="three-panel">
                  <div class="panel-title">
                    <div class="row">
                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/roll.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>

                      <div class="col-12 col-md-6 col-lg-6">
                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/orange_juice.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/pizza_max.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>

                        <NuxtLink to="/menu_details">
                          <div class="py-3">
                            <div class="d-flex">
                              <img
                                src="~assets/images/01.png"
                                class="rounded-3 img-fluid"
                                width="80px"
                                height="30px"
                                alt=""
                              />

                              <div class="justify-content-end mx-1">
                                <div class="menus_head">
                                  <p class="m-0 fs-6 mb-0">
                                    Chocolate Milkshake
                                  </p>
                                  <p
                                    class="mx-3 mb-0"
                                    style="
                                      color: #7d2883;
                                      font-weight: 700;
                                      font-size: 20px;
                                    "
                                  >
                                    $105
                                  </p>
                                </div>
                                <p
                                  class="rounded-cake py-1 px-1 m-0 text-secondary"
                                >
                                  Lorem ipsum dolor sit amet
                                </p>

                                <div class="d-flex flex-wrap">
                                  <button
                                    class="btn border border-1 rounded-pill px-2"
                                  >
                                    <div class="star5 px-2">
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span
                                        class="fa fa-star checked bg-yellow"
                                      ></span>
                                      <span class="fa fa-star bg-yellow"></span>
                                      <span class="fa fa-star"></span>
                                    </div>
                                  </button>
                                  <p
                                    class="mb-0 mt-1 ms-3 text-muted"
                                    style="font-size: 12px"
                                  >
                                    ( 454 reviews )
                                  </p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </NuxtLink>
                      </div>
                    </div>
                  </div>
                  <p></p>
                </div>
              </div>
            </div>

            <nav class="pagination-container w-100">
              <div
                class="pagination w-100 text-center d-flex justify-content-center align-items-center"
              >
                <a class="pagination-newer" href="#"
                  ><i
                    class="fas fa-angle-left"
                    style="color: black; font-size: 40px"
                  ></i
                ></a>
                <span class="pagination-inner">
                  <a href="#">1</a>
                  <a class="pagination-active" href="#">2</a>
                  <a href="#">3</a>
                </span>
                <a class="pagination-older" href="#"
                  ><i
                    class="fas fa-angle-right"
                    style="color: black; font-size: 40px"
                  ></i
                ></a>
              </div>
            </nav>
          </div>
          <!-- </div> -->
        </div>

        <div
          class="col-12 col-lg-3 uddin bg-white cord flex-end ps-0 ps-lg-3 ps-md-3 mt-2 ansab"
        >
          <p class="fs-5 m-auto mt-2 text-center text-lg-start">
            <b>Daily Trending Menus</b>
          </p>
          <p
            class="text-muted text-center text-lg-start"
            style="font-size: 12px"
          >
            Lorem Ipsum is simply dummy text
          </p>
          <NuxtLink to="/menu_details">
            <div class="mt-5 mb-3" style="border-bottom: 1px solid lightgrey">
              <div class="d-flex justify-content-around">
                <h6 class="text-secondary mt-2 fw-bold">#1</h6>
                <h5 class="star5">
                  <b>Chocolate Milkshake</b>
                  <div class="">
                    <p class="bg-purple py-2 fwb">
                      <b>$105</b>
                      <span class="text-muted">( 454 reviews )</span>
                      <!-- <p class="text-center  review "></p> -->
                    </p>
                  </div>
                </h5>
                <img
                  src="~assets/images/01.png"
                  class="d-flex justify-content-end mini_img mx-2 mt-0"
                  width="50px"
                  height="50px"
                  alt=""
                />
              </div>
            </div>
          </NuxtLink>

          <NuxtLink to="/menu_details">
            <div class="my-3" style="border-bottom: 1px solid lightgrey">
              <div class="d-flex justify-content-around">
                <h6 class="text-secondary mt-2 fw-bold">#2</h6>
                <h5 class="star5">
                  <b>Chocolate Milkshake</b>
                  <div class="">
                    <p class="bg-purple py-2 fwb">
                      <b>$105</b>
                      <span class="text-muted">( 454 reviews )</span>
                      <!-- <p class="text-center  review "></p> -->
                    </p>
                  </div>
                </h5>
                <img
                  src="~assets/images/02.png"
                  class="d-flex justify-content-end mini_img mx-2 mt-0"
                  width="50px"
                  height="50px"
                  alt=""
                />
              </div>
            </div>
          </NuxtLink>

          <NuxtLink to="/menu_details">
            <div class="my-3" style="border-bottom: 1px solid lightgrey">
              <div class="d-flex justify-content-around">
                <h6 class="text-secondary mt-2 fw-bold">#3</h6>
                <h5 class="star5">
                  <b>Chocolate Milkshake</b>
                  <div class="">
                    <p class="bg-purple py-2 fwb">
                      <b>$105</b>
                      <span class="text-muted">( 454 reviews )</span>
                      <!-- <p class="text-center  review "></p> -->
                    </p>
                  </div>
                </h5>
                <img
                  src="~assets/images/03.png"
                  class="d-flex justify-content-end mini_img mx-2 mt-0"
                  width="50px"
                  height="50px"
                  alt=""
                />
              </div>
            </div>
          </NuxtLink>

          <NuxtLink to="/menu_details">
            <div class="my-3">
              <div class="d-flex justify-content-around">
                <h6 class="text-secondary mt-2 fw-bold">#4</h6>
                <h5 class="star5">
                  <b>Chocolate Milkshake</b>
                  <div class="">
                    <p class="bg-purple py-2 fwb">
                      <b>$105</b>
                      <span class="text-muted">( 454 reviews )</span>
                      <!-- <p class="text-center  review "></p> -->
                    </p>
                  </div>
                </h5>
                <img
                  src="~assets/images/04.png"
                  class="d-flex justify-content-end mini_img mx-2 mt-0"
                  width="50px"
                  height="50px"
                  alt=""
                />
              </div>
            </div>
          </NuxtLink>
        </div>
      </div>
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
