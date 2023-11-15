<template>
  <section id="about">
    <div class="bg-news">
      <img src="~@/assets/img/rectangle.png" />
    </div>
    <v-container id="features">
      <div class="text-news">
        <v-row align="center" justify="center">
          <v-col cols="12" class="text-center">
            <h1 class="text-title-news">Latest News</h1>
            <h2 class="text-description-news">
              At elKopra we are committed to providing top-notcto cater to all your needs. Our team of dedicated professionals is passionate about delivering exceptional solutions that exceed expectation
            </h2>
          </v-col>
        </v-row>
      </div>
    </v-container>
  </section>
</template>

<style scoped>
#about {
  background-color: #4830B0;
}
.bg-news {
  position: absolute;
  z-index: 1;
  width: 100%;
}
.bg-news img {
  width: 100%;
  height: 500px;
}
</style>
