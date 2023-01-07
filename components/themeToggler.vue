<template>
    <div class="">
        <button @click="changeTheme()">
            <svg v-if="$colorMode.preference === 'dark'" xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="icon" width="4em"
                height="4em" viewBox="0 0 24 24" data-v-389e99a3="" data-v-97ee44f7="">
                <path fill="currentColor"
                    d="M21.64 13a1 1 0 0 0-1.05-.14a8.05 8.05 0 0 1-3.37.73a8.15 8.15 0 0 1-8.14-8.1a8.59 8.59 0 0 1 .25-2A1 1 0 0 0 8 2.36a10.14 10.14 0 1 0 14 11.69a1 1 0 0 0-.36-1.05Zm-9.5 6.69A8.14 8.14 0 0 1 7.08 5.22v.27a10.15 10.15 0 0 0 10.14 10.14a9.79 9.79 0 0 0 2.1-.22a8.11 8.11 0 0 1-7.18 4.32Z">
                </path>
            </svg>

            <svg v-else-if="$colorMode.preference === 'light'" xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="icon" width="2em"
                height="2em" viewBox="0 0 24 24" data-v-389e99a3="" data-v-97ee44f7="">
                <path fill="currentColor"
                    d="m5.64 17l-.71.71a1 1 0 0 0 0 1.41a1 1 0 0 0 1.41 0l.71-.71A1 1 0 0 0 5.64 17ZM5 12a1 1 0 0 0-1-1H3a1 1 0 0 0 0 2h1a1 1 0 0 0 1-1Zm7-7a1 1 0 0 0 1-1V3a1 1 0 0 0-2 0v1a1 1 0 0 0 1 1ZM5.64 7.05a1 1 0 0 0 .7.29a1 1 0 0 0 .71-.29a1 1 0 0 0 0-1.41l-.71-.71a1 1 0 0 0-1.41 1.41Zm12 .29a1 1 0 0 0 .7-.29l.71-.71a1 1 0 1 0-1.41-1.41l-.64.71a1 1 0 0 0 0 1.41a1 1 0 0 0 .66.29ZM21 11h-1a1 1 0 0 0 0 2h1a1 1 0 0 0 0-2Zm-9 8a1 1 0 0 0-1 1v1a1 1 0 0 0 2 0v-1a1 1 0 0 0-1-1Zm6.36-2A1 1 0 0 0 17 18.36l.71.71a1 1 0 0 0 1.41 0a1 1 0 0 0 0-1.41ZM12 6.5a5.5 5.5 0 1 0 5.5 5.5A5.51 5.51 0 0 0 12 6.5Zm0 9a3.5 3.5 0 1 1 3.5-3.5a3.5 3.5 0 0 1-3.5 3.5Z">
                </path>
            </svg>

            <svg v-else-if="$colorMode.preference === 'sepia'" class="icon" width="2em" height="2em" viewBox="0 0 256 256"><path fill="currentColor" d="M80 56V24a8 8 0 0 1 16 0v32a8 8 0 0 1-16 0Zm40 8a8 8 0 0 0 8-8V24a8 8 0 0 0-16 0v32a8 8 0 0 0 8 8Zm32 0a8 8 0 0 0 8-8V24a8 8 0 0 0-16 0v32a8 8 0 0 0 8 8Zm96 56v8a40 40 0 0 1-37.5 39.9a98 98 0 0 1-27 40.1H208a8 8 0 0 1 0 16H32a8 8 0 0 1 0-16h24.5A96.4 96.4 0 0 1 24 136V88a8 8 0 0 1 8-8h176a40 40 0 0 1 40 40Zm-48-24H40v40a80.3 80.3 0 0 0 45.1 72h69.8a80.3 80.3 0 0 0 41.9-49.9a1.4 1.4 0 0 0 .2-.6a77 77 0 0 0 3-21.5Zm32 24a24 24 0 0 0-16-22.6V136a92.9 92.9 0 0 1-1.2 15a24 24 0 0 0 17.2-23Z"/></svg>

            <svg v-else xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true"
                role="img" class="icon" width="2em" height="2em" viewBox="0 0 24 24" data-v-389e99a3=""
                data-v-97ee44f7="">
                <path fill="currentColor"
                    d="M19 3H5a3 3 0 0 0-3 3v8a3 3 0 0 0 3 3h6v2H7a1 1 0 0 0 0 2h10a1 1 0 0 0 0-2h-4v-2h6a3 3 0 0 0 3-3V6a3 3 0 0 0-3-3Zm1 11a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V6a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1Z">
                </path>
            </svg>
        </button>
    </div>
</template>


<script setup>
const colorMode = useColorMode()

function changeTheme() {
    if (colorMode.preference === 'dark') {
        colorMode.preference = 'light'
    }
    else if (colorMode.preference === 'light') {
        colorMode.preference = 'sepia'
    }
    else if (colorMode.preference === 'sepia') {
        colorMode.preference = 'system'
    }
    else if (colorMode.preference === 'system') {
        colorMode.preference = 'dark'
    }
}
</script>

<style>
.icon:hover {
    color: #00DC82;
}
</style>
