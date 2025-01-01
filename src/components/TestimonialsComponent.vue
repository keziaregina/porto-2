<template>
  <div class="dizme_tm_section">
    <div class="dizme_tm_testimonials">
      <div class="dizme_tm_main_title" data-align="center">
        <span style="color: #e7c0d4;">Testimonials</span>
        <h3 style="color: #eb96c1; font-weight: bold">What My Clients Say</h3>
        <!-- <p>
          Most common methods for designing websites that work well on desktop
          is responsive and adaptive design
        </p> -->
      </div>
      <div class="list_wrapper">
        <div class="total">
          <div class="in">
            <swiper
              :pagination="{ clickable: true, el: '.owl-dots' }"
              :modules="modules"
              class="owl-carousel owl-theme"
            >
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    Very professional and well organized. She created a step by step plan in Trello 
                    and completed the steps quickly. She has good management and makes 
                    quick progress. 
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <div
                      class="main"
                      data-img-url="/img/testimonials/ninedragonlabs-michael.jpg"
                    ></div>
                  </div>
                  <div class="detail">
                    <h3>Michael kravc</h3>
                    <span>Road to Virtuosity</span>
                  </div>
                </div>
              </swiper-slide>
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    Professional work has been done very well. The work is done with great
                    patience so that customer satisfaction is guaranteed. The value of the money
                    spent is very much paid off with very satisfying results.
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <div
                      class="main"
                      data-img-url="/img/testimonials/turai.png"
                    ></div>
                  </div>
                  <div class="detail">
                    <h3>Turai
                      </h3>
                    <span>Agrommunity</span>
                  </div>
                </div>
              </swiper-slide>
              <swiper-slide>
                <div class="icon" v-html="testimonialIcon"></div>
                <div class="text">
                  <p>
                    Talented and excellent developer in building applications with the latest
                    technology. Also, her communication with clients is very good and always
                    tries to satisfy the needs of clients. I highly recommend her with A++
                  </p>
                </div>
                <div class="short">
                  <div class="image">
                    <div
                      class="main"
                      data-img-url="/img/testimonials/samah.jpg"
                    ></div>
                  </div>
                  <div class="detail">
                    <h3>Samah
                      </h3>
                    <span>Jobsicle</span>
                  </div>
                </div>
              </swiper-slide>
            </swiper>
            <div class="owl-dots"></div>
          </div>
          <div class="left_details">
            <div
              class="det_image one wow fadeIn"
              data-wow-duration="1s"
              data-img-url="/img/testimonials/jude.jpg"
            ></div>
            <div
              class="det_image two wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.2s"
              data-img-url="/img/testimonials/michael.jpg"
            ></div>
            <div
              class="det_image three wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.4s"
              data-img-url="/img/testimonials/samah.jpg"
            ></div>
            <div
              class="det_image four wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.6s"
              data-img-url="/img/testimonials/turai.png"
            ></div>
            <span class="circle green animPulse"></span>
            <span class="circle yellow animPulse"></span>
            <span class="circle border animPulse"></span>
          </div>
          <div class="right_details">
            <div
              class="det_image one wow fadeIn"
              data-wow-duration="1s"
              data-img-url="/img/testimonials/ninedragonlabs-michael.jpg"
            ></div>
            <div
              class="det_image two wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.2s"
              data-img-url="/img/testimonials/ninedragonlabs-michael.jpg"
            ></div>
            <div
              class="det_image three wow fadeIn"
              data-wow-duration="1s"
              data-wow-delay="0.4s"
              data-img-url="/img/testimonials/turai.png"
            ></div>
            <span class="circle yellow animPulse"></span>
            <span class="circle purple animPulse"></span>
            <span class="circle border animPulse"></span>
          </div>
        </div>
      </div>
      <div class="brush_1 wow fadeInRight" data-wow-duration="1s">
        <img src="/img/brushes/testimonials/1.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import { testimonialIcon } from "@/svg";
import { Pagination } from "swiper";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
export default {
  name: "TestimonialsComponent",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      testimonialIcon,
    };
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>
