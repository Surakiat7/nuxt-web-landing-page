<template>
    <div class="w-full relative rounded-2xl overflow-hidden">
        <nuxt-img :src="coverImage" alt="Cover image" width="2280" class="w-full aspect-square object-cover rounded-2xl" />
        <span class="absolute top-2 right-2 px-2 rounded-full text-sm text-white bg-primary">
            {{ duration }}
        </span>
        <div
            class="absolute py-2 px-3 md:py-3 md:px-4 bottom-0 h-28 flex flex-col justify-between inset-x-0 bg-gradient-to-t from-zinc-950 bg-opacity-50 backdrop-filter backdrop-blur-sm">
            <h2 class="text-white font-semibold text-sm sm:text-base line-clamp-2">
                {{ title }}
            </h2>
            <div class="pt-2">
                <NuxtLink :to="href"
                    class="flex items-center text-white rounded-full p-0.5 pr-2 gap-2 text-sm border border-gray-100/20 w-max">
                    <span class="p-1 rounded-full bg-primary">
                        <svg xmlns="http://www.w3.org/2000/svg" fill='currentColor' viewBox="0 0 24 24" class='w-4 h-4'>
                            <path
                                d="M8,3V7H21l-2,7H8v2H18a1,1,0,0,1,0,2H7a1,1,0,0,1-1-1V4H4A1,1,0,0,1,4,2H7A1,1,0,0,1,8,3ZM6,20.5A1.5,1.5,0,1,0,7.5,19,1.5,1.5,0,0,0,6,20.5Zm9,0A1.5,1.5,0,1,0,16.5,19,1.5,1.5,0,0,0,15,20.5Z" />
                        </svg>
                    </span>
                    Shop now.
                </NuxtLink>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
const { title, href, duration, coverImage } = defineProps<{
    title: string,
    href: string,
    duration: string,
    coverImage: string
}>()
</script>