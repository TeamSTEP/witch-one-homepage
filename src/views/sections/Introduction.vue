<template>
    <section id="intro-page" class="w-full h-screen">
        <page-outline>
            <background-cover :src="require('@/assets/video/background.mp4')" />
            <div class="pt-10 md:pt-24">
                <div
                    class="container px-3 mx-auto my-auto flex flex-wrap flex-col md:flex-row items-center"
                >
                    <!--Left Col-->
                    <div
                        class="flex flex-col w-full md:w-2/5 justify-center items-center text-center absolute md:static"
                    >
                        <img
                            :src="require('@/assets/img/icon-512.png')"
                            class="w-full h-full px-5 mx-auto"
                            alt="logo"
                        />
                        <a
                            href="https://team-step.gitbook.io/witch-one-design-doc/"
                            target="_blank"
                        >
                            <button
                                class="mx-auto hover:underline gradient text-white font-bold rounded-full mt-24 md:my-6 py-4 px-8 shadow-lg focus:outline-none focus:shadow-outline transform transition hover:scale-105 duration-300 ease-in-out"
                            >
                                Learn More
                                <i class="fa fa-external-link" />
                            </button>
                        </a>
                    </div>

                    <!--Right Col-->
                    <div class="w-full md:w-3/5 py-6 items-center text-center z-10">
                        <h1 class="my-4 text-8xl font-bold leading-tight text-white">Witch One</h1>
                        <!--text divider-->
                        <div class="w-full mb-4">
                            <div
                                class="h-1 mx-auto gradient w-64 opacity-25 my-0 py-0 rounded-t"
                            ></div>
                        </div>
                        <p class="leading-normal text-2xl mb-8 text-white text-center">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam at
                            ipsum eu nunc commodo posuere et sit amet ligula.
                        </p>
                    </div>
                </div>
            </div>
        </page-outline>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import PageOutline from '@/components/PageOutline.vue';
import BackgroundCover from '@/components/BackgroundCover.vue';

export default defineComponent({
    components: {
        PageOutline,
        BackgroundCover,
    },
});
</script>

<style lang="scss">
#intro-page {
    h1 {
        font-family: 'Annie Use Your Telescope', Helvetica, Arial, cursive;
        text-shadow: 2px 2px 5px black;
    }
}
</style>
