<template>
  <div>
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
      <!-- <button
        class="btn my-4 text-lg-start bg-purple-d-a text-white button-radius-a px-3"
        type="submit"
      >
        Back
      </button> -->
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

            <!-- <form id="contactForm" data-sb-form-api-token="API_TOKEN">
                        <div class="mb-3 ">
                            
                            
                        </div>
                        <div class="mb-3 ">
                            <label class="form-label " for="dish">Dish</label>
                            <input class="form-control" id="dish" type="text" placeholder="Prepopulated"
                                data-sb-validations="" />
                        </div>
                        <div class="mb-3   ">
                            <label class="form-label" for=""></label>
                            <input class="form-control  " id="" type="text" placeholder="Spice"
                                data-sb-validations="" />
                            <label class="form-label" for=""></label>
                            <input class="form-control  mx-1" id="" type="text" placeholder="Portion"
                                data-sb-validations="" />
                        </div>
                        <div class="mb-3 d-flex   ">
                            <label class="form-label" for=""></label>
                            <input class="form-control  " id="" type="text" placeholder="Value"
                                data-sb-validations="" />
                            <label class="form-label" for=""></label>
                            <input class="form-control  mx-1" id="" type="text" placeholder="Mayne Factor"
                                data-sb-validations="" />
                        </div>
                        <div class="mb-3 d-flex   ">
                            <label class="form-label" for=""></label>
                            <input class="form-control " id="" type="text" placeholder="Overall"
                                data-sb-validations="" />

                        </div>

                        <div class="mb-3 ">
                      
                        </div>
                        <div class="d-none" id="submitSuccessMessage">
                            <div class="text-center mb-3">

                            </div>
                        </div>

                    </form> -->
            <hr class="my-5" />
            <div class="col-12 text-center">
              <div class="star-3 text-lg-center pt-5">
                <span class="fa fa-star checked bg-yellow fs-1"></span>
                <span class="fa fa-star checked bg-yellow fs-1"></span>
                <span class="fa fa-star checked bg-yellow fs-1"></span>
                <span class="fa fa-star bg-yellow fs-1"></span>
                <span class="fa fa-star fs-1"></span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
