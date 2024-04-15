<template>
  <div class="flex flex-col overflow-hidden">
    <div
      class="sm:bg-left-center relative min-h-screen w-screen overflow-hidden logo-screen:h-full"
    >
      <div
        class="relative sm-pb-[134px] lg-pb-[87px] flex h-full flex-col items-center pb-[170px] pt-[75px] 2xl:pt-[106px]"
      >
        <video class="bg-video" :src="VideoBg" autoplay muted loop></video>
        <div class="bg-video-darken"></div>
        <div class="relative mb-10 flex flex-auto flex-col items-center z-10">
          <img
            :src="MainLogo"
            alt="Logo Tacticool"
            class="mb-10 h-[90px] w-[270px] object-contain sm:h-[114px] sm:w-[342px] xl:h-[142px] xl:w-[428px]"
          />
          <div
            class="max-w-[667px] text-center text-xl font-black leading-[28px] text-white md:text-2xl md:leading-[34px]"
          >
            One of the most intense shooters, featuring an unparalleled
            isometric view, realistic physics, cars, and destructible
            environment!
          </div>
        </div>

        <BaseButton class="relative z-10" />
      </div>
      <BaseFooter />
    </div>
  </div>
</template>

<script setup lang="ts">
import { useTitle } from "@vueuse/core";
import BaseButton from "../components/BaseButton.vue";
import MainLogo from "../assets/main-logo.png";
import BaseFooter from "../components/footer/BaseFooter.vue";
import VideoBg from "../assets/main-bg.mp4"
import {onMounted} from "vue";

const title = useTitle();
title.value = "Tacticool";

</script>

<style scoped></style>
