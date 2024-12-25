<template>
    <div :class="carousel.type">
        <div class="left flex flex-col text-2xl bg-zinc-800 p-2 rounded-lg shadow-md my-auto py-10 items-center">
            <div class="text-gray-400 ">
                {{ carousel.title }}
            </div>
            <div class="text-lg mt-5">
                {{ carousel.description }}
            </div>
            <div class="text-lg mt-2 flex items-center">
                <a v-if="carousel.buttonType === 'demo'" class="demo-button" :href="carousel.link" target="_blank">
                    <p>Demo</p>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="w-6 h-6 mr-2">
                        <path stroke-linecap="round"
                            d="M15.75 10.5l4.72-4.72a.75.75 0 011.28.53v11.38a.75.75 0 01-1.28.53l-4.72-4.72M4.5 18.75h9a2.25 2.25 0 002.25-2.25v-9a2.25 2.25 0 00-2.25-2.25h-9A2.25 2.25 0 002.25 7.5v9a2.25 2.25 0 002.25 2.25z" />
                    </svg>
                </a>
                <a v-else class="demo-button" :href="carousel.link" target="_blank">
                    <p>Link</p>
                    <svg class="w-6 h-6 mr-2" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="24"
                        height="24" fill="none" viewBox="0 0 24 24">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M18 14v4.833A1.166 1.166 0 0 1 16.833 20H5.167A1.167 1.167 0 0 1 4 18.833V7.167A1.166 1.166 0 0 1 5.167 6h4.618m4.447-2H20v5.768m-7.889 2.121 7.778-7.778" />
                    </svg>

                </a>
            </div>
        </div>
        <div :id="`carousel-${carousel.id}`" class="right carousel slide relative lg:w-2/3" data-bs-ride="carousel">
            <div v-if="carousel.images.length > 1">
                <div class="carousel-indicators absolute right-0 bottom-0 left-0 flex justify-center p-0 mb-4">
                    <button v-for="(image, index) in carousel.images" :key="index" type="button"
                        :data-bs-target="`#carousel-${carousel.id}`" :data-bs-slide-to="index"
                        :class="{ active: (index === 0) }" :aria-label="`Slide ${index + 1}`"></button>
                </div>
            </div>
            <div class="carousel-inner relative w-full overflow-hidden">
                <div v-for="(image, index) in carousel.images" :key="index"
                    class="carousel-item relative float-left w-full" :class="{ active: index === 0 }">
                    <div class="relative overflow-hidden bg-no-repeat bg-cover" style="background-position: 50%;">
                        <img :src="image.link" class="block w-full" />
                        <div
                            class="absolute top-0 right-0 bottom-0 left-0 w-full h-full overflow-hidden bg-fixed bg-black opacity-20">
                        </div>
                        <div class="carousel-caption hidden md:block absolute text-center">
                            <h5 class="text-xl">{{ image.description }}</h5>
                        </div>
                    </div>
                </div>
            </div>
            <div v-if="carousel.images.length > 1">
                <button
                    class="carousel-control-prev absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline left-0"
                    type="button" :data-bs-target="`#carousel-${carousel.id}`" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon inline-block bg-no-repeat" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button
                    class="carousel-control-next absolute top-0 bottom-0 flex items-center justify-center p-0 text-center border-0 hover:outline-none hover:no-underline focus:outline-none focus:no-underline right-0"
                    type="button" :data-bs-target="`#carousel-${carousel.id}`" data-bs-slide="next">
                    <span class="carousel-control-next-icon inline-block bg-no-repeat" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'ProjectComponent',
    props: {
        carousel: Object
    }
}
</script>