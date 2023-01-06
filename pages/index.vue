<template>
  <div class="intro py-12 px-8 sm:py-7 sm:px-40">
    <h2 class="text-[50px] sm:text-[90px] font-bold flex">Hello. 
      <span>
        <img class="hello_gif sm:h-24 sm:w-24 h-[50px] w-[50px]"
          src="https://camo.githubusercontent.com/e8e7b06ecf583bc040eb60e44eb5b8e0ecc5421320a92929ce21522dbc34c891/68747470733a2f2f6d656469612e67697068792e636f6d2f6d656469612f6876524a434c467a6361737252346961377a2f67697068792e676966">
        </span>
    </h2>
    <h3 class="text-[1.5rem] sm:text-[34px] pt-4">My name is <span class="font-bold text-transparent bg-clip-text bg-gradient-to-r from-[#00dc82] to-[#36e4da]">Tejas Magade</span></h3>
  </div>
</template>

<script setup>

</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Rubik:300,500,700');

.intro {
  font-family: "Rubik", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  /* font-size: calc(10px + 0.33vw); */
  -webkit-font-smoothing: antialiased;
}

.intro::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.intro {
  -ms-overflow-style: none;
  /* IE and Edge */
  scrollbar-width: none;
  /* Firefox */
}

</style>
