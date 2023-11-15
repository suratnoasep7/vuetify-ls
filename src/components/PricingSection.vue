<template>
  <section id="pricing" class="pb-8">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-card class="card">
            <v-row>
            
            <v-col cols="7">
              <h1 class="text-card">Subscribe news letter</h1>
              <h2 class="text-description-card">Using a combination of technology, process and talents we focus on our users needs and help to accelerate their business at any scale. We deliver consistent </h2>
              <v-row no-gutters>
                <v-col cols="4">
                  <v-text-field solo flat style="border-radius: 0" placeholder="Input email" />
                </v-col>
                <v-col cols="4">
                  <v-btn tile depressed dark large class="btn-send">
                    Send Email
                  </v-btn>
                </v-col>
              </v-row>
              <h3 class="text-description-card-detail">This site is protected by reCAPTCHA and the Google Privacy Policy and Terms of Service apply.</h3>
            </v-col>
            <v-col cols="5">
              <div class="img-card-detail">
                <img src="~@/assets/img/passion_4.png" />
              </div>
              
            </v-col>

            </v-row>
            
            
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    
  </section>
</template>

<style lang="scss">
#pricing {
  background-color: #4830B0;
  padding: 80px 0px;
}
.card {
  background: #6444F0 !important;
  box-shadow: none !important;
  padding: 20px;
}
.text-card {
  color: #FFF;
  font-size: 40px;
  font-style: normal;
  font-weight: 700;
  line-height: 40px;
}
.text-description-card {
  color: #FFF;
  font-family: DM Sans;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 40px;
  margin-bottom: 10px;
}
.v-input__slot {
  border-top-left-radius: 25px !important;
  border-bottom-left-radius: 25px !important;
  width: 120% !important;
}
.btn-send {
  background: #EC9109 !important;
  border: 1px solid #EC9109 !important;
  padding: 6px 12px !important;
  height: 48px !important;
}
.text-description-card-detail {
  margin: 0px 0px;
  font-size: 12px;
font-style: normal;
font-weight: 400;
line-height: 24px;
color: #fff;
}
.img-card-detail {
  position: relative;
}
.img-card-detail img {
  width: 100% !important;
  position: absolute;
  top: -134px;
}
.v-btn {
  border-radius: 25px !important;
}
$main_color: #283e79;

ul {
  font-size: 13px;
  line-height: 1.5em;
  margin: 5px 0 15px;
  padding: 0;

  li {
    list-style: none;
    position: relative;
    padding: 0 0 0 20px;
  }

  li {
    &::before {
      content: "";
      position: absolute;
      left: 0;
      top: 5px;
      width: 10px;
      height: 10px;
      background-color: $main_color;
      border-radius: 50%;
      -moz-border-radius: 50%;
      -webkit-eeborder-radius: 50%;
    }
  }
}
</style>

<style scoped>
.header {
  background-color: #283e79;
  color: white;
}

.circle1 {
  border-radius: 50%;
  width: 150px;
  height: 150px;
  background-color: #f0f8ff;
  display: flex;
  align-items: center;
  justify-content: center;
}

.circle2 {
  border-radius: 50%;
  width: 100px;
  height: 100px;
  background-color: #e0effc;
  display: flex;
  align-items: center;
  justify-content: center;
}

.flex-center {
  display: flex;
  align-items: center;
  justify-content: center;
}

.svg-border-rounded svg {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  color: #f4f7f5;
  z-index: -1;
}

#pricing {
  z-index: 0;
}

.content {
  z-index: 1;
}

svg {
  overflow: hidden;
}

section {
  position: relative;
}

</style>

<script>
export default {
  data: () => ({
    planos: [
      {
        title: "Básico",
        price: "R$100,00",
        img: "f1.png",
        features: [
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 1",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 2",
          },
          {
            icon: {
              text: "mdi-cancel",
              color: "red",
            },
            text: "Feature 3",
          },
          {
            icon: {
              text: "mdi-cancel",
              color: "red",
            },
            text: "Feature 4",
          },
        ],
      },
      {
        title: "Padrão",
        price: "R$150,00",
        img: "f2.png",
        features: [
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 1",
            color: "success",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 2",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 3",
            color: "success",
          },
          {
            icon: {
              text: "mdi-cancel",
              color: "red",
            },
            text: "Feature 4",
          },
        ],
      },
      {
        title: "Premium",
        price: "R$250,00",
        img: "f3.png",
        features: [
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 1",
            color: "success",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 2",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 3",
            color: "success",
          },
          {
            icon: {
              text: "mdi-check",
              color: "success",
            },
            text: "Feature 4",
            color: "success",
          },
        ],
      },
    ],
  }),
  computed: {
    size() {
      const size = {md: "large", xl: "x-large"}[
          this.$vuetify.breakpoint.name
          ];
      return size ? {[size]: true} : {};
    }
  },
};
</script>