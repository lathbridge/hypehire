<template>
  <q-layout class="mainlayout">
    <div class="bluebg text-white q-my-none">
      <div class="q-pr-lg" style="display: flex; justify-content: flex-end">
        <img
          alt="whitedash"
          src="~assets/white.svg"
          style="width: 30px; height: 60px"
        />
      </div>

      <div class="q-px-lg q-pb-sm q-pt-none">
        <img
          alt="Quasar logo"
          src="~assets/logo.svg"
          style="width: 114px; height: 21px"
        />
      </div>

      <div class="row q-pa-lg">
        <div>
          <h1 class="text-h3 text-weight-bolder" style="cursor: pointer">
            고의 실력을 가진 외국인 인재를 찾고 계신가요?
          </h1>
          <p class="text-h6 text-weight-bold">
            법률 및 인사관리 부담없이 1주일 이내에 원격으로 채용해보세요.
          </p>
        </div>

        <!-- carousel pics -->

        <q-carousel
          v-model="slide"
          transition-prev="slide-right"
          transition-next="slide-left"
          swipeable
          animated
          control-color="white"
          padding="none"
          arrows
          height="100%"
          width="100%"
          class="rounded-borders bg-transparent"
          style="
            display: flexbox;
            justify-content: center;
            align-items: center;
            margin: auto;
          "
        >
          <q-carousel-slide :name="1" class="">
            <img class="" src="~assets/cardd.svg" />
          </q-carousel-slide>
          <q-carousel-slide :name="2" class="">
            <img class="" src="~assets/cardd.svg" />
          </q-carousel-slide>
          <q-carousel-slide :name="3" class="">
            <img class="" src="~assets/cardd.svg" />
          </q-carousel-slide>
        </q-carousel>
      </div>

      <!-- check icons  -->
      <div class="q-px-lg q-pb-lg">
        <div>
          <img alt="Quasar logo" src="~assets/checkbox.svg" class="q-mr-sm" />

          <img alt="Quasar logo" src="~assets/checkbox2.png" />
        </div>
        <div>
          <img alt="Quasar logo" src="~assets/checkbox3.png" class="q-mr-lg" />
          <img alt="Quasar logo" src="~assets/checkbox4.png" />
        </div>
        <h5 class="text-h6" style="text-decoration: underline; color: yellow">
          개발자가 필요하신가요?
        </h5>
      </div>
    </div>

    <!-- white bg section -->
    <div class="secondbackground q-pa-lg">
      <div>
        <img
          alt="Quasar logo"
          src="~assets/logo2.svg"
          style="width: 200px; height: 100%"
        />
      </div>
      <div>
        <h5
          style="
            line-height: 21px;
            font-weight: 900;
            font-size: 14px;
            color: #343741;
          "
        >
          우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
        </h5>
        <h5
          style="
            line-height: 20px;
            font-weight: 900;
            font-size: 13px;
            margin: 0px;
            padding: 0px;
            color: #5e626f;
          "
        >
          010-0000-0000
        </h5>

        <h5
          style="
            line-height: 20px;
            font-weight: 900;
            font-size: 13px;
            color: #5e626f;
            margin: 0px;
            padding: 0px;
          "
        >
          aaaaa@naver.com
        </h5>
      </div>

      <!-- Cards below -->
      <div class="q-pt-md flex-start">
        <img
          alt="Quasar logo"
          src="~assets/card1.png"
          style="height: 100%; width: 160px"
          class="q-ma-sm"
        />
        <img
          alt="Quasar logo"
          src="~assets/card2.svg"
          style="height: 100%; width: 160px"
          class="q-ma-sm"
        />
      </div>
      <div>
        <img
          alt="Quasar logo"
          src="~assets/card3.png"
          style="height: 100%; width: 160px"
          class="q-ma-sm"
        />
        <img
          alt="Quasar logo"
          src="~assets/card4.svg"
          style="height: 100%; width: 160px"
          class="q-ma-sm"
        />
      </div>

      <!-- Footer part -->
      <div class="q-pt-md">
        <img
          alt="Quasar logo"
          src="~assets/layer1.svg"
          style="height: 100%; width: 350px"
          class="q-pb-lg"
        />

        <img
          alt="Quasar logo"
          src="~assets/layer2.svg"
          style="height: 100%; width: 200px"
          class="q-pb-lg"
        />

        <img
          alt="Quasar logo"
          src="~assets/foot.svg"
          style="height: 100%; width: 350px"
          class="q-pb-lg"
        />

        <h5
          style="
            line-height: 20px;
            font-weight: 900;
            font-size: 13px;
            color: #5e626f;
            margin: 0px;
            padding: 0px;
          "
        >
          ⓒ 2023 Hyperhire
        </h5>
      </div>
    </div>
  </q-layout>
</template>

<script setup>
defineOptions({
  name: "MainLayout",
});

import { ref } from "vue";

const slide = ref(1);
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

* {
  font-family: "Poppins", sans-serif;
}
.mainlayout {
  max-width: 500px;
  margin: auto auto;
}

.secondbackground {
  background-color: #fbfbfb;
}

.bluebg {
  background-image: url("../assets/bluemain.svg");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
