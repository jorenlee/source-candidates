<template>
  <div>
    <div class="mx-auto mb-20 lg:w-9/12">
      <div>
        <img class="object-cover mx-auto" :src="tes_banner" alt="" />
      </div>
      <div class="mt-10 mx-auto px-20">
        <video width="1200" height="300" controls class="mx-auto">
            <source :src="fullVideo" type="video/mp4" />
            <source :src="fullVideo" type="video/ogg" />
          </video>
      </div>
      <br />
      <div class="lg:grid lg:grid-cols-2 lg:gap-10 lg:justify-evenly">
        <div
          class="relative lg:w-10/12 w-11/12 mx-auto lg:mb-0 mb-10"
          v-for="(t, i) in tes"
          :key="i"
        >
          <video width="500" height="500" controls>
            <source :src="t.bannerPic" type="video/mp4" />
            <source :src="t.bannerPic" type="video/ogg" />
          </video>
        </div>
      </div>
      <div>
         <img class="object-cover w-10/12 my-10 mx-auto" :src="smile_banner" alt="" />
      </div>
      <div class="lg:grid lg:grid-cols-2 lg:gap-10 lg:justify-evenly">
       
        <div
          class="relative lg:w-10/12 w-11/12 mx-auto lg:mb-0 mb-10"
          v-for="(s, i) in smile"
          :key="i"
        >
          <img class="object-cover" :src="s.bannerPic" alt="" />
        </div>
      </div>
      <h1
        class="
          text-center
          mb-14
          text-2xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-r
          from-green-400
          to-green-600
          lg:w-11/12
          w-4/5
          mx-auto
          mt-20
        "
      >

        
        <span class="">SOURCE List of All Candidates</span>
      </h1>
      <div class="lg:grid lg:grid-cols-2 lg:gap-10 lg:justify-evenly mt-10">
       
        <div
          class="relative lg:w-10/12 w-11/12 mx-auto lg:mb-0 mb-10"
          v-for="(src, i) in source"
          :key="i"
        >
          <img class="object-cover" :src="src.bannerPic" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Posters",
  components: {},
  data() {
    return {
      tes: [
        {
          bannerPic: require("@/assets/img/posters/tes/ruel.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/emman.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/kissy.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/lucy.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/neil.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/keith.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/aliza.mp4"),
        },
        {
          bannerPic: require("@/assets/img/posters/tes/wena.mp4"),
        },
      ],
      smile: [
        {
          bannerPic: require("@/assets/img/posters/smile/jessa.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/harlie.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/ryle.png"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/cathy.png"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/ruffa.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/piolo.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/mark.png"),
        },
        {
          bannerPic: require("@/assets/img/posters/smile/heart.png"),
        },
      ],
      source: [
        {
          bannerPic: require("@/assets/img/posters/source/jessa.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/ruel.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/emman.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/harlie.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/ryle.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/kissy.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/cathy.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/lucy.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/neil.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/ruffa.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/piolo.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/keith.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/mark.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/aliza.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/heart.jpg"),
        },
        {
          bannerPic: require("@/assets/img/posters/source/wena.jpg"),
        }
      ],
      tes_banner: require("@/assets/img/posters/tes/campaign-banner.jpg"),
      smile_banner: require("@/assets/img/posters/smile/smile_banner.gif"),
      fullVideo: require("@/assets/img/posters/tes/TES_Video.mp4"),
    };
  },
};
</script>
