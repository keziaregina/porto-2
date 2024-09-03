<template>
  <div class="dizme_tm_section" id="portfolio">
    <div class="dizme_tm_portfolio">
      <div class="container">
        <div class="dizme_tm_main_title" data-align="center">
          <!-- <span>Portfolio</span> -->
          <h3>My Portfolio</h3>
          <p>
            Explore my portfolio, where my skills in full stack development come to life. These projects highlight my expertise in technologies like Laravel, Python, and NextJs, demonstrating my dedication to creating innovative solutions.
            <!-- Explore my portfolio, where my skills in full stack development come to life. These projects highlight my expertise in technologies like Laravel, Python, and NextJs, demonstrating my dedication to creating innovative solutions. -->
          </p>
        </div>
        <div class="portfolio_filter">
          <ul>
            <li>
              <a
                class="c-pointer"
                :class="activeNavcls === '1' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '1')"
                data-filter="*"
                >All</a
              >
            </li>
            <li>
              <a  
                class="c-pointer"
                :class="activeNav === '2' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '2')"
                data-filter=".web"
                >Web</a
              >
            </li>
            <li>
              <a
                class="c-pointer"
                :class="activeNav === '3' ? 'current' : ''"
                @click.prevent="() => (this.activeNav = '3')"
                data-filter=".mobile"
                >Mobile</a
              >
            </li>
          </ul>
        </div>
        <div class="dizme_tm_portfolio_titles"></div>
        <div class="portfolio_list wow fadeInUp" data-wow-duration="1s">
          <ul class="gallery_zoom grid">
            <li class="mobile grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="mobile"
                >
                  <!-- <a
                    class="popup-mobile"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/23.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>Sales Tracking</h3>
                  <span>Indosat</span>
                </div>
              </div>
            </li>
            <li class="web grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="web"
                >
                  <!-- <a
                    class="popup-vimeo"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/19.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>Marketing Apps
                  </h3>
                  <span>Indosat Ooredoo
                  </span>
                </div>
              </div>
            </li>
            <li class="mobile grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="mobile"
                >
                  <!-- <a
                    class="mfp-iframe audio"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/22.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>Waste Cycling Apps
                  </h3>
                  <span>Indonesia Port</span>
                </div>
              </div>
            </li>
            <li class="mobile grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="mobile"
                >
                  <!-- <a
                    class="zoom"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-56.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/24.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>E-Book Apps</h3>
                  <span>Islamic State University
                  </span>
                </div>
              </div>
            </li>
            <li class="web grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="web"
                >
                  <!-- <a
                    class="zoom"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/21.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>Freelance Jobs Posting
                  </h3>
                  <span>IFreelance
                  </span>
                </div>
              </div>
            </li>
            <li class="web grid-item">
              <div class="inner">
                <div
                  class="entry dizme_tm_portfolio_animation_wrap"
                  
                  data-category="web"
                >
                  <!-- <a
                    class="portfolio_popup"
                    href="#"
                  > -->
                    <img src="/img/thumbs/42-34.jpg" alt="" />
                    <div class="main" data-img-url="/img/portfolio/20.jpg"></div>
                  <!-- </a> -->
                </div>
                <div class="mobile_title">
                  <h3>Crane Monitoring
                  </h3>
                  <span>Indonesia Port
                  </span>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
      <div class="brush_1 wow zoomIn" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/1.png" alt="" />
      </div>
      <div class="brush_2 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/portfolio/2.png" alt="" />
      </div>
    </div>
  </div>
  <MagnificPopUpVue
    :modal="modal"
    :close="closeModal"
    :name="name"
    :src="src"
  />
  <div :class="`${active === 1 ? '' : 'hidden_content'}`">
    <ModalBox :close="close">
      <div class="popup_details">
        <div class="top_image">
          <img src="img/thumbs/4-2.jpg" alt="" />
          <div
            class="main"
            data-img-url="img/portfolio/6.jpg"
            style="background-image: url('img/portfolio/6.jpg')"
          ></div>
        </div>
        <div class="portfolio_main_title">
          <h3>Global Evolution</h3>
          <span><a href="#">Detail</a></span>
          <div></div>
        </div>
        <div class="main_details">
          <div class="textbox">
            <p>
              We live in a world where we need to move quickly and iterate on
              our ideas as flexibly as possible.
            </p>
            <p>
              Mockups are useful both for the creative phase of the project -
              for instance when you're trying to figure out your user flows or
              the proper visual hierarchy - and the production phase when they
              phase when they will represent the target product. Building
              mockups strikes the ideal balance ease of modification.
            </p>
          </div>
          <div class="detailbox">
            <ul>
              <li>
                <span class="first">Client</span>
                <span>Alvaro Morata</span>
              </li>
              <li>
                <span class="first">Category</span>
                <span><a href="#">Detail</a></span>
              </li>
              <li>
                <span class="first">Date</span>
                <span>March 07, 2021</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="additional_images">
          <ul>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/1.jpg"
                    style="background-image: url('img/portfolio/1.jpg')"
                  ></div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/2.jpg"
                    style="background-image: url('img/portfolio/2.jpg')"
                  ></div>
                </div>
              </div>
            </li>
            <li>
              <div class="list_inner">
                <div class="my_image">
                  <img src="img/thumbs/4-2.jpg" alt="" />
                  <div
                    class="main"
                    data-img-url="img/portfolio/3.jpg"
                    style="background-image: url('img/portfolio/3.jpg')"
                  ></div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </ModalBox>
  </div>
</template>

<script>
import MagnificPopUpVue from "./popup/MagnificPopUp.vue";
import ModalBox from "./popup/ModalBox.vue";
export default {
  name: "PortfolioComponent",
  data() {
    return {
      activeNav: "1", // props
      name: "",
      src: "",
      modal: false,
      // Content
      active: 0,
    };
  },
  mounted() {
    let Isotope = require("isotope-layout");
    setTimeout(() => {
      let iso = new Isotope(".gallery_zoom", {
        itemSelector: ".grid-item",
        //    layoutMode: "fitRows",
        percentPosition: true,
        masonry: {
          columnWidth: ".grid-item",
        },
        animationOptions: {
          duration: 750,
          easing: "linear",
          queue: false,
        },
      });
      let filterFns = {
        // show if number is greater than 50
        numberGreaterThan50: function (itemElem) {
          let number = itemElem.querySelector(".number").textContent;
          return parseInt(number, 10) > 50;
        },
        // show if name ends with -ium
        ium: function (itemElem) {
          let name = itemElem.querySelector(".name").textContent;
          return name.match(/ium$/);
        },
      };
      // bind filter button click filter main funtion
      let filtersElem = document.querySelector(".portfolio_filter ul");
      filtersElem.addEventListener("click", function (event) {
        if (event.target.getAttribute("data-filter")) {
          let filterValue = event.target.getAttribute("data-filter");
          filterValue = filterFns[filterValue] || filterValue;
          iso.arrange({ filter: filterValue });
        }
      });
    }, 1000);
  },
  methods: {
    onClick(name, src) {
      this.name = name;
      this.src = src;
      this.modal = true;
    },
    closeModal() {
      this.modal = false;
      this.name = "";
      this.src = "";
    },
    close() {
      this.active = 0;
    },
  },
  components: { MagnificPopUpVue, ModalBox },
};
</script>
