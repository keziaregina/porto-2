<template>
  <div class="dizme_tm_header">
    <div class="container">
      <div class="inner">
        <div class="logo">
          <a href="#" style="text-decoration: none;color: black;  font-weight: bold;">
            Kezia Regina
          </a>
        </div>
        <div class="menu">
          <ul class="anchor_nav">
            <li class="current"><a href="#home">Home</a></li>
            <!-- <li><a href="#about">About</a></li> -->
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#service">Service</a></li>
            <li><a href="https://medium.com/@keziaregina28">Blog</a></li>
            <li><a href="https://wa.me/6285601487041">WhatsApp</a></li>
            <li><a href="https://www.linkedin.com/in/keziaeci/">LinkedIn</a></li>
            <li><a href="https://www.upwork.com/freelancers/~01d5648c3acbeed168?viewMode=1">Upwork</a></li>
            <li><a href="mailto:keziaregina28@gmail.com">Email Me</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderVue",
  props: {
    dark: { type: Boolean },
  },
};
</script>
