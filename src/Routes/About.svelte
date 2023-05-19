<main>
  <!-- Navigation bar  -->
  <div
    class="col-md-12 text-left px-4 py-2 background_of_navbar text_for_mobile"
  >
    <a style="text-decoration: none; color: #212529;" href="/">
      <h5><b><i class="fas fa-arrow-left" /> Page Title</b></h5>
    </a>
  </div>

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
    <div class="container px-md-5 px-2 pb-3">
      <div class="col-md-12 bg-white">
        <div class="col-md-12 text-center">
          <img
            class="img-fluid image_banner_width pt-4 pb-4"
            src="../Images/banner.jpg"
            alt=""
          />
        </div>
        <div class="col-md-12 px-md-5 px-2 py-5">
          <span class="badge bg-success">Live</span>
          <h1>Pittsburgh Collaborative x Goodr Grocery at Gideons Kindezi</h1>
          <h2>05/01/2023 15:30</h2>
          <h6>
            The Pittsburgh Collaborative has partnered with Goodr to bring a
            free supplemental food resource to Kindezi at Gideons.
          </h6>
          <div class="row pb-2">
            <div class="col-md-1 col-1 text-center">
              <span class="icon_marker"
                ><i class="fas fa-map-marker-alt" /></span
              >
            </div>
            <div class="col-md-11 col-11 pl-0">
              <h5>Gideons Elementary School</h5>
              <h6>897 Welch Street Southwest Atlanta, GA 30310</h6>
            </div>
          </div>
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3318.173014052291!2d-84.40800462445632!3d33.73034198465926!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x88f5030e0cb9163d%3A0xc72663fb465c74ff!2s897%20Welch%20St%20SW%2C%20Atlanta%2C%20GA%2030310%2C%20USA!5e0!3m2!1sen!2s!4v1682680874007!5m2!1sen!2s"
            title=""
            width="100%"
            height="450"
            style="border:0;"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          />
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  main {
    overflow-x: hidden;
    background-color: #f7f8f8;
  }
  .icon_marker {
    font-size: 200%;
    color: #1f5a3f;
  }

  .image_banner_width {
    width: 70%;
  }

  .img_logo_style {
    width: 15%;
  }

  .background_of_navbar {
    background-color: #fff;
    border-bottom: 1px solid lightgray;
  }

  .navbar {
    display: none;
  }
  .text_for_mobile {
    display: none;
  }

  @media only screen and (max-width: 600px) {
    .background_of_navbar {
      display: none;
    }
    .text_for_mobile {
      display: block;
    }
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
  }
</style>
