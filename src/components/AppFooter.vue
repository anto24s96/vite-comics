<script>
export default {
    name: "AppFooter",
    data() {
        return {};
    },
};
</script>
<template lang="">
  <div id="bg-banner">
    <div class="container d-flex space-between">
      <div class="d-flex" id="main-container-footer-list">
        <div class="list-footer-container">
          <ul>
            <li class="text-white">DC COMICS</li>
            <li class="text-gray">Characters</li>
            <li class="text-gray">Comics</li>
            <li class="text-gray">Movies</li>
            <li class="text-gray">TV</li>
            <li class="text-gray">Games</li>
            <li class="text-gray">Video</li>
            <li class="text-gray">News</li>
          </ul>

          <ul>
            <li class="text-white">SHOP</li>
            <li class="text-gray">Shop DC</li>
            <li class="text-gray">Shop DC Collectibles</li>
          </ul>
        </div>

        <div class="list-footer-container">
          <ul>
            <li class="text-white">DC</li>
            <li class="text-gray">Terms Of Use</li>
            <li class="text-gray">Privacy policy (New)</li>
            <li class="text-gray">Ad Choice</li>
            <li class="text-gray">Advertising</li>
            <li class="text-gray">Jobs</li>
            <li class="text-gray">Subscriptions</li>
            <li class="text-gray">Talent Workshop</li>
            <li class="text-gray">CPSC Certificates</li>
            <li class="text-gray">Ratings</li>
            <li class="text-gray">Shop Help</li>
            <li class="text-gray">Contact Us</li>
          </ul>
        </div>

        <div class="list-footer-container">
          <ul>
            <li class="text-white">SITES</li>
            <li class="text-gray">DC</li>
            <li class="text-gray">MAD Magazine</li>
            <li class="text-gray">DC Kids</li>
            <li class="text-gray">Dc Universe</li>
            <li class="text-gray">DC Power Visa</li>
          </ul>
        </div>
      </div>

      <div class="logo-footer-container">
        <img src="../assets/img/dc-logo-bg.png" alt="logo_background" />
      </div>
    </div>
  </div>

  <div class="bg-black-2">
    <div class="container d-flex align-items space-between" id="footer-icons">
      <span id="sign-button" class="text-white"> SIGN-UP-NOW! </span>

      <ul class="footer-list-icons d-flex align-items">
        <li>FOLLOW US</li>
        <li><img src="../assets/img/footer-facebook.png" alt="fb" /></li>
        <li><img src="../assets/img/footer-twitter.png" alt="twitter" /></li>
        <li><img src="../assets/img/footer-youtube.png" alt="yt" /></li>
        <li><img src="../assets/img/footer-pinterest.png" alt="pinterest" /></li>
        <li><img src="../assets/img/footer-periscope.png" alt="periscope" /></li>
      </ul>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

#bg-banner {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    height: 370px;
    position: relative;

    #main-container-footer-list {
        padding-top: 50px;

        .list-footer-container {
            margin-right: 40px;

            ul {
                list-style-type: none;
            }

            ul li:first-child {
                margin-bottom: 10px;
                font-weight: 600;
                font-size: 16px;
            }

            ul li:last-child {
                margin-bottom: 20px;
            }

            li {
                margin: 5px;
                font-size: 13px;
            }
        }
    }

    .logo-footer-container {
        img {
            position: relative;
            width: 550px;
            top: -90px;
        }
    }
}

.bg-black-2 {
    background-color: #303030;
    position: relative;
    z-index: 999;
    padding: 30px 0;

    #sign-button {
        border: 2px solid $blue_primary;
        padding: 10px;
    }

    .footer-list-icons {
        list-style-type: none;

        li:first-child {
            color: $blue_primary;
            font-size: 18px;
            margin-right: 10px;
            font-weight: 600;
        }

        img {
            width: 30px;
            margin: 0 10px;
        }
    }
}
</style>
