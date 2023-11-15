<template>
  <section id="download">
    <v-container>
      <v-row align="center" justify="center">
        <v-col cols="12">
          <v-row align="center" justify="center">
            
            <v-col cols="12" class="white--text text-left">
              <h1 class="text-download-news">Lorem ipsum dolot amet lorem ipsum</h1>
              <h2 class="text-description-download-news">
                Our <span>Passion</span> What We Do.
              </h2>
            </v-col>
            <v-col cols="4" class="align-center passion">
              <v-col cols="12" align="center" justify="center">
                <img src="~@/assets/img/passion_1.png" />
              </v-col>
              
              <p class="text-center text-percentage">
                98%
              </p>
              <p class="text-center text-description">Possitive Feedback</p>
            </v-col>
            <v-col cols="4" class="align-center">
              <v-col cols="12" align="center" justify="center">
                <img src="~@/assets/img/passion_2.png" />
              </v-col>
              <p class="text-center text-percentage">
                120
              </p>
              <p class="text-center text-description">Enthusiastic Fulltime Employee</p>
            </v-col>
            <v-col cols="4" class="align-center">
              <v-col cols="12" align="center" justify="center">
                <img src="~@/assets/img/passion_3.png" />
              </v-col>
              <p class="text-center text-percentage">
                20
              </p>
              <p class="text-center text-description">Projects Completed</p>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
#download {
  background-color: #4830B0;
  padding: 80px 0px;
}
.text-download-news {
  color: #FFF;
  text-align: center;
  font-family: DM Sans;
  font-size: 24px;
  font-style: normal;
  font-weight: 500;
  line-height: 32px;
  margin-bottom: 40px;
}
.text-description-download-news {
  text-align: center;
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 40px;
  margin-bottom: 40px;
}
.text-description-download-news span {
  color: #EC9109;
}
.text-percentage {
  color: #FFF;
  font-size: 60px;  
  font-style: normal;
  font-weight: 700;
  line-height: 40px;
  margin-bottom: 20px;
}
.text-description {
  color: #FFF;
  font-size: 24px;
  font-style: normal;
  font-weight: 500;
  line-height: 40px;
  margin-bottom: 20px;
}
.passion img {
  text-align: center;
}
</style>