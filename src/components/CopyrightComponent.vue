<template>
  <div class="dizme_tm_section">
    <div class="dizme_tm_copyright">
      <div class="container">
        <div class="inner">
          <div class="left wow fadeInLeft" data-wow-duration="1s">
            <p>
              Developed with love by
              <a href="https://www.linkedin.com/in/keziaeci/" target="_blank"
                >Kezia Regina</a
              >
              &copy; {{ new Date().getFullYear() }}
            </p>
          </div>
          <div class="right wow fadeInRight" data-wow-duration="1s">
            <ul>
              <!-- <li><a href="#">Terms &amp; Condition</a></li> -->
              <li><a href="https://wa.me/6285601487041">WhatsApp</a></li>
              <li><a href="https://www.linkedin.com/in/keziaeci/">LinkedIn</a></li>
              <li><a href="https://www.upwork.com/freelancers/~01d5648c3acbeed168?viewMode=1">Upwork</a></li>
              <li><a href="mailto:keziaregina28@gmail.com">Email Me</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CopyrightComponent",
  components: {},
};
</script>
