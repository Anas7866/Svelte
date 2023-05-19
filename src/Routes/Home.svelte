<script>
  import Map from "../Components/googlemaps.svelte";
</script>

<main>
  <!-- Navigation bar  -->
  <div class="col-md-12 text-center py-2 background_of_navbar">
    <img
      class="img-fluid img_logo_style"
      src="../Images/logo.png"
      alt="image_crashed"
    />
  </div>

  <!-- content  -->
  <div class="col-md-12 overflow_dashboard mt-4">
    <div class="col-md-12 padding_right_feedmore py-4">
      <div class="col-md-12 py-5 border_color_feedmore">
        <div class="col-md-12 text-center">
          <p class="line_height">Feed More.</p>
          <p class="font_size_waste_less">Waste Less</p>
        </div>
        <div class="col-md-12 px-md-5 px-2">
          <p class="mb-3 genrel_text_color"><b>Location</b></p>
          <Map />
        </div>
        <div class="col-md-12 px-md-5 px-2">
          <div class="row">
            <div class="col-md-4">
              <p class="genrel_text_color"><b>Start Date</b></p>
              <input
                type="date"
                class="form-control input_form_style"
                aria-describedby="basic-addon2"
              />
            </div>
            <div class="col-md-4 pt-md-0 pt-4">
              <p class="genrel_text_color"><b>End Date</b></p>
              <input
                type="date"
                class="form-control input_form_style"
                aria-describedby="basic-addon2"
              />
            </div>
            <div class="col-md-4 pt-md-0 pt-4">
              <p class="genrel_text_color"><b>Distance</b></p>
              <select
                class="form-select input_form_style"
                aria-label="Default select example"
              >
                <option selected>10 Miles</option>
                <option value="1">20 Miles</option>
                <option value="2">30 Miles</option>
                <option value="3">40 Miles</option>
              </select>
            </div>
            <div class="col-md-4 pt-4">
              <p class="font_upcoming_events">Upcoming Events:</p>
            </div>
            <div class="col-md-12">
              <div
                class="col-md-12 mt-2 py-3 px-4 border_cards_upcoming_events"
              >
                <a
                  style="text-decoration: none; color: #212529;"
                  href="#/about"
                >
                  <div class="row">
                    <div class="col-md-1 text-center">
                      <p class="mb-0"><b>3.31 Miles</b></p>
                      <span class="icon_marker"
                        ><i class="fas fa-map-marker-alt" /></span
                      >
                    </div>
                    <div class="col-md-11">
                      <h4 class="mb-0 big_text_heading pb-2">
                        Pittsburgh Collaborative x Goodr Grocery at Gideons
                        Kindezi
                      </h4>
                      <h6 class="mb-0">05/01/2023 15:30:00</h6>
                      <p class="mb-0 address">
                        897 Welch Street Southwest Atlanta, GA 30310
                      </p>
                    </div>
                  </div>
                </a>
              </div>
              <div
                class="col-md-12 mt-2 py-3 px-4 border_cards_upcoming_events"
              >
                <div class="row">
                  <div class="col-md-1 text-center">
                    <p class="mb-0"><b>3.31 Miles</b></p>
                    <span class="icon_marker"
                      ><i class="fas fa-map-marker-alt" /></span
                    >
                  </div>
                  <div class="col-md-11">
                    <h4 class="mb-0 big_text_heading pb-2">
                      Pittsburgh Collaborative x Goodr Grocery at Gideons
                      Kindezi
                    </h4>
                    <h6 class="mb-0">05/01/2023 15:30:00</h6>
                    <p class="mb-0 address">
                      897 Welch Street Southwest Atlanta, GA 30310
                    </p>
                  </div>
                </div>
              </div>
              <div
                class="col-md-12 mt-2 py-3 px-4 border_cards_upcoming_events"
              >
                <div class="row">
                  <div class="col-md-1 text-center">
                    <p class="mb-0"><b>3.31 Miles</b></p>
                    <span class="icon_marker"
                      ><i class="fas fa-map-marker-alt" /></span
                    >
                  </div>
                  <div class="col-md-11">
                    <h4 class="mb-0 big_text_heading pb-2">
                      Pittsburgh Collaborative x Goodr Grocery at Gideons
                      Kindezi
                    </h4>
                    <h6 class="mb-0">05/01/2023 15:30:00</h6>
                    <p class="mb-0 address">
                      897 Welch Street Southwest Atlanta, GA 30310
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- navbar for mobile  -->
    <div class="navbar">
      <div class="row text-center">
        <div class="col-md-3 col-3">
          <span class="icons_car"><i class="fas fa-car" /></span>
        </div>
        <div class="col-md-3 col-3">
          <span class="icons_car"><i class="fas fa-hamburger" /></span>
        </div>
        <div class="col-md-3 col-3">
          <span class="icons_car"><i class="fas fa-shapes" /></span>
        </div>
        <div class="col-md-3 col-3">
          <span class="icons_car"><i class="fas fa-user-circle" /></span>
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  main {
    overflow-x: hidden;
  }

  .icon_marker {
    font-size: 260%;
    color: #1f5a3f;
  }
  .border_cards_upcoming_events {
    box-shadow: 1px 1px 4px 4px lightgray;
    border-radius: 5px;
    cursor: pointer;
  }
  .address {
    color: #8f9ca2;
  }
  .img_logo_style {
    width: 15%;
  }

  .background_of_navbar {
    background-color: #fff;
    box-shadow: 0 8px 8px -4px #dbe1e0;
  }

  .navbar {
    display: none;
  }

  .input_form_style:focus {
    box-shadow: none;
    outline: none;
    border: 1px solid #86b941;
  }
  .genrel_text_color {
    color: #575f72;
  }

  .line_height {
    line-height: 20px;
    text-decoration: underline;
    text-underline-offset: 13px;
    font-size: 260%;
    color: #1f5a3f;
  }
  .font_size_waste_less {
    font-size: 260%;
    color: #86b941;
  }
  .font_upcoming_events {
    font-size: 220%;
    color: #86b941;
  }
  .border_color_feedmore {
    box-shadow: 1px 1px 4px 4px lightgray;
    border-radius: 10px;
  }
  .padding_right_feedmore {
    padding-right: 3%;
    padding-left: 3%;
  }

  @media only screen and (max-width: 600px) {
    .icons_car {
      font-size: 160%;
      color: #575f72;
    }
    .img_logo_style {
      width: 35%;
    }
    .navbar {
      overflow: hidden;
      position: fixed;
      bottom: 0;
      width: 100%;
      display: block;
      border-top: 1px solid #575f7287;
      background-color: white;
    }
    .line_height {
      line-height: 20px;
      text-decoration: underline;
      text-underline-offset: 13px;
      font-size: 160%;
      color: #1f5a3f;
    }
    .font_size_waste_less {
      font-size: 160%;
      color: #86b941;
    }
    .font_upcoming_events {
      font-size: 120%;
      color: #86b941;
    }
  }
</style>
