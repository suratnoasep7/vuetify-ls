<template>
  <section id="hero">
    <v-parallax height="750" class="bg-home">
      <v-row align="center" justify="center">
        <v-col cols="12">
          <v-row align="center" justify="center">
            <v-col cols="5" md="5" xl="5">
              <h1 class="mb-4 title-home">Generate <span>New</span> <br /> Digital Cooperation</h1>
              <h2 class="title-description-home mb-4">
                We design and build solutions by connecting ideas <br /> and 
                technologhy to solve problems and get new ideas to <br /> 
                business lifecycle.
              </h2>
              <v-btn
                rounded
                outlined
                large
                dark
                @click="$vuetify.goTo('#features')"
                class="mt-5 btn-get-started"
              >
                Get Started
                
              </v-btn>
              
            </v-col>

            <v-col cols="4" md="4" xl="4">
              <img src="~@/assets/img/home-header.png" />
            </v-col>

          </v-row>
        </v-col>
      </v-row>
    </v-parallax>
    
  </section>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
      videoId: "i8IvvHJssWE",
      features: [
        {
          img: require("@/assets/img/icon2.png"),
          title: "Design Limpo",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          img: require("@/assets/img/icon1.png"),
          title: "Dados Seguros",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
        {
          img: require("@/assets/img/icon3.png"),
          title: "Código Aberto",
          text: "Lorem ipsum dolor sit amet consectetur adipisicing elit.",
        },
      ],
    };
  },
  watch: {
    dialog(value) {
      if (!value) {
        this.pause();
      }
    },
  },
  methods: {
    ready(event) {
      this.player = event.target;
    },
    playing(event) {
      // The player is playing a video.
    },
    change() {
      // when you change the value, the player will also change.
      // If you would like to change `playerVars`, please change it before you change `videoId`.
      // If `playerVars.autoplay` is 1, `loadVideoById` will be called.
      // If `playerVars.autoplay` is 0, `cueVideoById` will be called.
      this.videoId = "another video id";
    },
    stop() {
      this.player.stopVideo();
    },
    pause() {
      this.player.pauseVideo();
    },
  },
};
</script>

<style lang="scss">
.circle {
  stroke: white;
  stroke-dasharray: 650;
  stroke-dashoffset: 650;
  -webkit-transition: all 0.5s ease-in-out;
  opacity: 0.3;
}
.btn-get-started {
  background: #EC9109;
  border: 1px solid #EC9109;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 40px;
  color: #fff;
  text-transform: capitalize;
  padding: 6px 24px !important;
}
.title-home {
  font-size: 72px !important;
  font-style: normal !important;
  font-weight: 700 !important;
  line-height: 100px !important;
}
.text-news {
  position: relative;
  z-index: 3;
  margin: 12% 0px;
}
.text-title-news {
  color: #090227;
  text-align: center;
  font-family: DM Sans;
  font-size: 48px;
  font-style: normal;
  font-weight: 700;
  line-height: 40px; 
  margin-bottom: 20px;
}
.text-description-news {
  color: #A1A1A1;
text-align: center;
font-family: DM Sans;
font-size: 18px;
font-style: normal;
font-weight: 400;
line-height: 32px;
}
.v-parallax__image {
  opacity: 0 !important;
}
.title-description-home {
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: 40px;
  color: #fff;
}
.title-home span {
  color: #EC9109;
}
.bg-home {
  background: #4830B0;
}

.playBut {
  /*  border: 1px solid red;*/
  display: inline-block;
  -webkit-transition: all 0.5s ease;

  .triangle {
    -webkit-transition: all 0.7s ease-in-out;
    stroke-dasharray: 240;
    stroke-dashoffset: 480;
    stroke: white;
    transform: translateY(0);
  }

  &:hover {
    .triangle {
      stroke-dashoffset: 0;
      opacity: 1;
      stroke: white;
      animation: nudge 0.7s ease-in-out;

      @keyframes nudge {
        0% {
          transform: translateX(0);
        }
        30% {
          transform: translateX(-5px);
        }
        50% {
          transform: translateX(5px);
        }
        70% {
          transform: translateX(-2px);
        }
        100% {
          transform: translateX(0);
        }
      }
    }

    .circle {
      stroke-dashoffset: 0;
      opacity: 1;
    }
  }
}
</style>

<style>
.btn-play {
  transition: 0.2s;
}
.svg-border-waves .v-image {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 3rem;
  width: 100%;
  overflow: hidden;
}

#hero {
  z-index: 0;
}
.svg-border-waves img {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  margin-bottom: -2px;
  z-index: -1;
}

.card {
  min-height: 300px;
  padding: 10px;
  transition: 0.5s ease-out;
}

.card .v-image {
  margin-bottom: 15px;
  transition: 0.75s;
}

.card h1 {
  margin-bottom: 10px;
}

.zoom-efect {
  transform: scale(1.1);
}

.up {
  transform: translateY(-20px);
  transition: 0.5s ease-out;
}
</style>

<style>
section {
  position: relative;
}
</style>
