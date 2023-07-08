<script lang="ts" setup>
</script>

<template>
  <header>
    <div class="flex justify-between items-center max-w-8xl mx-auto mx-auto px-8 sm:py-1 sm:px-40 py-1">
      <!-- <img src="~/assets/signature.svg" height="50px" width="50px"> -->
      <BaseLogo />
      <div class="flex items-center">
        <nav aria-label="Main Menu" class="opacity-75">
          <ul class="flex sm:space-x-10 space-x-1 items-center">
            <li>
              <NuxtLink to="#" class="hover:text-[#01DC84]">
                <span class="inline-block pr-2 invisible sm:visible">
                  <svg width="18" height="18" viewBox="0 0 24 24">
                    <g fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                      stroke-width="1.5">
                      <path d="M7 18h7m-7-4h1m-1-4h3M7 2h9.5L21 6.5V19" />
                      <path
                        d="M3 20.5v-14A1.5 1.5 0 0 1 4.5 5h9.752a.6.6 0 0 1 .424.176l3.148 3.148A.6.6 0 0 1 18 8.75V20.5a1.5 1.5 0 0 1-1.5 1.5h-12A1.5 1.5 0 0 1 3 20.5Z" />
                      <path d="M14 5v3.4a.6.6 0 0 0 .6.6H18" />
                    </g>
                  </svg>
                </span>Blog
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="#" class="hover:text-[#01DC84]"><span class="inline-block pr-2 invisible sm:visible">
                  <svg width="18" height="18" viewBox="0 0 24 24">
                    <path fill="currentColor"
                      d="M1 11h3v2H1v-2m18.1-7.5L17 5.6L18.4 7l2.1-2.1l-1.4-1.4M11 1h2v3h-2V1M4.9 3.5L3.5 4.9L5.6 7L7 5.6L4.9 3.5M10 22c0 .6.4 1 1 1h2c.6 0 1-.4 1-1v-1h-4v1m2-16c-3.3 0-6 2.7-6 6c0 2.2 1.2 4.2 3 5.2V19c0 .6.4 1 1 1h4c.6 0 1-.4 1-1v-1.8c1.8-1 3-3 3-5.2c0-3.3-2.7-6-6-6m1 9.9V17h-2v-1.1c-1.7-.4-3-2-3-3.9c0-2.2 1.8-4 4-4s4 1.8 4 4c0 1.9-1.3 3.4-3 3.9m7-4.9h3v2h-3v-2Z" />
                  </svg>
                </span>Projects</NuxtLink>
            </li>
            <li :title="$colorMode.value + ' Theme'" class="pl-0 pt-2 text-[#01DC84]">
              <themeToggler />
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<style>
header {
  border-style: none;
  backdrop-filter: blur(10px);
  position: sticky;
  top: 0;
  width: 100%;
  z-index: 50;
}

nav .icon {
  width: 1.5rem;
  height: 1.5rem;
}

/* @media (max-width: 768px) {
  nav .icon {
    display: none !important;
  }
} */
</style>