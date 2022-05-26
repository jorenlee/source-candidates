 <template>
  <div>
     <div class="mx-auto mb-20 lg:w-9/12">
        <div class="lg:grid lg:grid-cols-2 lg:gap-10 lg:justify-evenly">
          <div
            class="relative lg:w-10/12 w-11/12 mx-auto lg:mb-0 mb-10"
            v-for="(poster, i) in posters"
            :key="i"
          >
             <img
               class="rounded-full object-cover"
               :src="poster.bannerPic"
               alt=""
             />
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
        posters: [
          {
            bannerPic: require("@/assets/posters/jessa.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/andres.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/harlie.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/emman.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/ryle.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/kissy.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/cathy.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/lucy.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/abby.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/ruffa.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/piolo.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/keith.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/mark.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/aliza.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/heart.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/wena.jpg"),
          },
          {
            bannerPic: require("@/assets/posters/ruel.jpg"),
          },
        ],
      };
    },
  }
</script>