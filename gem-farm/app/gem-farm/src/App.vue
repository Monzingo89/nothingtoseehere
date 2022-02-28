<template>
  <div class="relative h-full min-h-screen">
    <TheNavBar />
    <div class="pt-10 px-10 flex justify-center align-middle">
      <p class="text-6xl pt-3 px-1 mt-1 text-white bold">GENTIE PROPERTY MANAGER</p>
    </div>
    <div class="italic mt-5 text-center"></div>

    <div class="p-10">
      <router-view />
    </div>

    <div class="pt-10"></div>
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar';
import TheFooter from '@/components/gem-farm/TheFooter';
import TheCat from '@/components/gem-farm/TheCat';
export default {
  components: { TheCat, TheFooter, TheNavBar },
};
</script>

<style>
body {
  background-image: url('./assets/background.png');
  position: center;
}
* {
  font-family: 'Playfair Display';
}
input[type='radio']:checked + span {
  @apply text-black;
}
</style>
