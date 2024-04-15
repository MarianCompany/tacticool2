<template>
  <button
    @click="onBtnClick"
    class="bg-btn-bg mt-[280px] flex h-[53px] items-center justify-center whitespace-nowrap border-2 border-yellow bg-footer bg-contain bg-center bg-no-repeat px-8 text-xl font-bold uppercase text-white transition duration-150 hover:scale-105 sm:mt-[263px] md:h-20 md:px-12 md:text-[26px] lg:mt-[300px] xl:mt-[220px]"
  >
    FREE DOWNLOAD
  </button>
</template>

<script setup>
defineOptions({
  name: "BaseButton",
});
const onBtnClick = () => {
  window.__GEM.detectAndDownload(
    "0.2002591",
    "https://static.gc.my.games/exe/TacticoolLoader.exe",
  );
};
</script>

<style lang="scss" scoped></style>
