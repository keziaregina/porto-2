<template>
  <div class="dizme_tm_section" id="home">
    <div class="dizme_tm_hero">
      <div
        class="background"
        :data-img-url="`/img/slider/3.png`"
      ></div>
      <div class="container">
        <div class="content">
          <div class="details">
            <div class="hello">
              <h3 class="orangeText">Hello, I'm</h3>
            </div>
            <div class="name">
              <h3>Kezia Regina</h3>
            </div>
            <div class="job">
              <p>
                A Fullstack Developer From
                Indonesia
              </p>
            </div>
            <div class="text">
              <p>
                A Fullstack Developer with 3 years of experience in Web Development.
                I've successfully delivered 150+ projects, specializing in crafting robust web applications and custom solutions.
              </p>
            </div>
            <div class="button">
              <div class="dizme_tm_button">
                <a class="anchor"  href="https://wa.me/6285601487041"><span>WhatsApp</span></a>
              </div>
            </div>
          </div>
          <div class="avatar">
            <div class="image">
              <img src="/img/slider/avatar-2.png" alt="" />
              <span
                class="skills illustrator anim_moveBottom"
                v-html="laravel"
              ></span>
              <span class="skills photoshop anim_moveBottom" v-html="js"></span>
              <span class="skills figma anim_moveBottom" v-html="html"></span>
            </div>
          </div>
        </div>
      </div>
      <div class="dizme_tm_down">
        <a class="anchor" href="#portfolio" v-html="dark ? mouseDark : mouse">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import { ai, figma,js,html, laravel, mouse, mouseDark, ps } from "../svg";
export default {
  name: "HomeComponent",
  data() {
    return { ai, ps,laravel,js,html, figma, mouse, mouseDark };
  },
  props: {
    dark: { type: Boolean },
  },
};
</script>
