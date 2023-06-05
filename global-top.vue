<script setup lang="ts">
const date = new Date().getFullYear().toLocaleString('fr-FR')
</script>

<template>
    <header v-if="$slidev.nav.currentLayout === 'cover'" absolute top-0 left-0 right-0 p-2><img src="/hoppr-logo.png" class="h-8" alt="HoppR Logo" /></header>
    <Scroll />
    <footer v-if="$slidev.nav.currentLayout !== 'about-me'">
        <div absolute bottom-0 p-2 flex flex-row flex-items-center flex-justify-around>
            <div>
                <a href="https://sunny-tech.io/" target="_blank"><img h-8 mr-4 src="/event-logo.png" alt="Event logo" /></a>
            </div>
            <div>
                <p mt text-2>© {{ date }}</p>
            </div>
        </div>
        <!-- <div   text-sm p-2>
            {{ date }}
        </div> -->
        <div absolute bottom-0 left-0 right-0 text-center text-sm p-2 >
            <a hover:text-light-blue-500  href="http://twitter.com/mderoullers"
                    target="_blank">@mderoullers</a>
        </div>
        <div v-if="$slidev.nav.currentLayout !== 'cover'" absolute bottom-0 left-230 right-0 text-sm p-2>
            <SlideCurrentNo />/
            <SlidesTotal />
        </div>
    </footer>
</template>