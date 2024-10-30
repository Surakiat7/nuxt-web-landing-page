<template>
    <div
        class="lg:p-1 relative h-auto flex flex-col lg:rounded-2xl lg:bg-box-bg lg:shadow-lg lg:shadow-box-shadow lg:border lg:border-box-border">
        <div class="relative h-max min-h-max">
            <nuxt-img :src="coverImage" alt="Cover image" width="280"
                class="w-full h-32 sm:h-36 md:h-40 lg:h-48 rounded-xl object-cover" />
            <span class="absolute top-2 right-2 px-2 rounded-full text-sm text-white bg-primary">
                {{ duration }}
            </span>
        </div>
        <div class="lg:px-2 pt-2 lg:pb-4 xl:px-4 md:pt-4  h-full flex flex-col justify-between">
            <div class="h-full">
                <h2
                    class="font-semibold text-base md:text-lg lg:text-xl line-clamp-2 md:line-clamp-3 text-primary dark:text-secondary">
                    {{ title }}
                </h2>
            </div>
            <div class="pt-3 sm:pt-5 min-h-max h-max">
                <NuxtLink :to="href"
                    class="flex relative group items-center text-white px-5 py-2 bg-primary gap-1 text-sm w-max rounded-full">
                    <span
                        class="absolute inset-0 rounded-full group-hover:scale-105 origin-center transition-all ease-in-out bg-primary dark:bg-zinc-800">

                    </span>
                    <span class="relative flex items-center dark:text-zinc-200 gap-3">
                        <svg xmlns="http://www.w3.org/2000/svg" fill='currentColor' viewBox="0 0 24 24" class='w-6 h-6'>
                            <path
                                d="M8,3V7H21l-2,7H8v2H18a1,1,0,0,1,0,2H7a1,1,0,0,1-1-1V4H4A1,1,0,0,1,4,2H7A1,1,0,0,1,8,3ZM6,20.5A1.5,1.5,0,1,0,7.5,19,1.5,1.5,0,0,0,6,20.5Zm9,0A1.5,1.5,0,1,0,16.5,19,1.5,1.5,0,0,0,15,20.5Z" />
                        </svg>
                        Shop now.
                    </span>
                </NuxtLink>
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
const { title, href, duration, coverImage, category, createdAt, description } = defineProps<{
    title: string,
    href: string,
    duration: string,
    coverImage: string,
    category: string,
    createdAt: string,
    description: string
}>()
</script>