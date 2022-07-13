<script>
import { RouterLink } from 'vue-router'
export default {
  name: 'Navbar',
  data() {
    return {
      isCollapsed: false
    }
  },
  methods: {
    toggleMenu() {
      this.isCollapsed = !this.isCollapsed;
    }
  }
}
</script>

<style lang="scss">
.mr-auto, .mx-auto {
  margin-right: auto !important;
}

.navbar {
  //background-color: #8caddb;
  //background-color: #8eaedc;
  .nav-item.dropdown-hover {
    position: relative;

    &:hover {
      .hover_menu {
        display: block;
      }
    }

    .hover_menu {
      position: absolute;
      top: 40px;
      left: 50%;
      background: #1F262C;
      border-radius: 30px;
      color: #fff;
      padding: 40px 40px 20px 40px;
      transform: translateX(-50%);
      width: 1086px;
      display: none;

      &:before {
        content: "";
        width: 0;
        height: 0;
        border-left: 8px solid transparent;
        border-right: 8px solid transparent;
        border-bottom: 10px solid #1F262C;
        position: absolute;
        top: -10px;
        left: 50%;
        transform: translateX(-50%);
      }

      .menu_contain {
        h2 {
          color: #657D93;
          font-weight: 400;
          font-size: 18px;
          line-height: 17px;
          text-transform: uppercase;
          padding: 0 15px;
        }

        .menu_box {
          padding: 10px 15px;
          margin-bottom: 20px;

          &.active, &:hover {
            background: rgba(59, 73, 86, 0.5);
            border-radius: 4px;
          }

          h3 {
            color: #E1F0FD;
            font-weight: 600;
            font-size: 16px;
            line-height: 19px;
            margin-bottom: 5px;
          }

          p {
            font-weight: 400;
            font-size: 14px;
            line-height: 17px;
            color: #657D93;
            margin-bottom: 0;
          }
        }
      }
    }
  }

  a {
    font-weight: 600;
    font-size: 14px;
    line-height: 17px;
  }

  @media (min-width: 992px) {
    .navbar-nav .nav-link {
      padding-right: 30px;
      padding-left: 30px;
    }
    .navbar-brand {
      margin-right: 40px;
    }
  }

}

.nav-colored-blue {
  background-color: #165ca1;
}

.nav-colored {
  background-color: #444d56;
}

.nav-trans {
  background-color: transparent;
}
</style>

<template>
  <nav id="navbarFix" class="navbar fixed-top navbar-expand-lg navbar-dark">
    <div class="container">
      <a class="navbar-brand" href="#banner"><img src="@/assets/images/logo.png" alt=""></a>
      <button class="navbar-toggler" type="button" @click="toggleMenu()"
              aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <RouterLink class="nav-link" to="/">Home</RouterLink>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#info-container">What we are</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#featured-container">Service</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about-us-container">Contact</a>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" to="/about">About</RouterLink>
          </li>
          <li class="nav-item dropdown-hover">
            <a class="nav-link" href="#">More <img src="@/assets/images/polygon.png" alt=""></a>
            <div class="hover_menu">
              <div class="row">
                <div class="col-md-3 col-6">
                  <div class="menu_contain">
                    <h2>Financial Services</h2>
                    <div class="menu_box active">
                      <h3>TJex.fund</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                    <div class="menu_box">
                      <h3>TJex.trade</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                    <div class="menu_box">
                      <h3>TJex.digital</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-3 col-6">
                  <div class="menu_contain">
                    <h2>Tools</h2>
                    <div class="menu_box">
                      <h3>TJex.help</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                    <div class="menu_box">
                      <h3>TJex.ai</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-3 col-6">
                  <div class="menu_contain">
                    <h2>Hrm & Reit</h2>
                    <div class="menu_box">
                      <h3>TJex.org</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                    <div class="menu_box">
                      <h3>TJex.estate</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                  </div>
                </div>
                <div class="col-md-3 col-6">
                  <div class="menu_contain">
                    <h2>Crm</h2>
                    <div class="menu_box">
                      <h3>TJex.cloud</h3>
                      <p>Lorem ipsum dolor sit amet</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </li>
        </ul>
        <ul class="navbar-nav full-right">
          <li class="nav-item active">
            <a class="nav-link" href="#">Language: English</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>