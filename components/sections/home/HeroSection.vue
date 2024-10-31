<template>
    <section class="relative w-full">
        <div class="absolute top-0 inset-x-0 h-64 flex items-start">
            <div
                class="h-24 w-2/3 bg-gradient-to-br bg-primary opacity-20 blur-2xl dark:from-secondary dark:invisible dark:opacity-40">
            </div>
            <div
                class="h-20 w-3/5 bg-gradient-to-r bg-primary opacity-10 blur-2xl dark:from-secondary dark:opacity-40">
            </div>
        </div>
        <AtomsContainer class-name='realtive'>
            <div aria-hidden="true" class="absolute inset-y-0 w-44 left-0 hidden dark:flex">
                <div
                    class="h-full md:h-1/2 lg:h-full w-full bg-primary opacity-10 dark:blur-2xl dark:from-secondary dark:opacity-20">
                </div>
            </div>
            <div
                class="grid lg:grid-cols-2 gap-10 xl:gap-14 relative pt-24 lg:max-w-none max-w-2xl md:max-w-3xl mx-auto">
                <div class="lg:py-6">
                    <div class="text-center lg:text-left">
                        <span class="px-2 py-1 rounded-md bg-zinc-200 dark:bg-zinc-700 text-primary dark:text-secondary">Discover Your Perfect
                            Pair of Glasses with OWNDAYS Labs</span>
                        <h1 class="text-zinc-800 pt-4 dark:text-white font-bold text-4xl md:text-5xl lg:text-6xl">
                            Explore our exclusive<br> collection of <span
                                class="text-transparent bg-clip-text bg-gradient-to-br from-primary to-secondary">Pair
                                eyewear</span>
                            tailored to fit every styles.
                        </h1>
                    </div>

                    <p class="text-zinc-600 dark:text-zinc-300 pt-8 text-center lg:text-left mx-auto max-w-xl">
                        At OWNDAYS Labs, we bring you the latest in eyewear fashion and technology. From classic frames
                        to innovative designs, find the perfect pair that suits your style and enhances your vision.
                    </p>

                    <div class="flex items-center gap-3 pt-9 flex-col sm:flex-row sm:w-max sm:mx-auto lg:mx-0">
                        <AtomsLinkBtn href="#" variant="primary" class="w-full sm:w-max flex justify-center">
                            Shop Now
                        </AtomsLinkBtn>
                    </div>
                    <div class="pt-8 lg:pt-10 w-max mx-auto lg:mx-0">
                        <div class="flex items-center text-center flex-col sm:flex-row gap-4 sm:gap-0">
                            <div class="flex items-center">
                                <img src="/jp-flag.png" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-zinc-200 dark:border-zinc-400 object-cover">
                                <img src="/th-flag.png" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-zinc-200 dark:border-zinc-400 object-cover -ml-2.5">
                                <span
                                    class="w-10 h-10 rounded-full border-2 border-zinc-200 dark:border-zinc-400 bg-body-color flex items-center justify-center text-xs text-zinc-300 object-cover -ml-2.5">
                                    10+
                                </span>
                            </div>
                            <div class="pl-2 text-zinc-600 dark:text-zinc-200">
                                "OWNDAYS has offices countries worldwide."
                            </div>
                        </div>
                    </div>
                </div>
                <div class="lg:h-full  hidden md:flex">

                    <div
                        class="flex w-full h-96 min-h-[24rem] lg:min-h-[none] lg:w-full lg:h-full items-center relative">
                        <div
                            class="absolute z-0 top-1/2  -translate-y-1/2 w-5/6 right-0 h-[calc(80%+20px)] bg-gradient-to-tr opacity-25 from-primary to-pink-300 dark:from-secondary dark:to-primary blur-2xl">
                        </div>
                        <div
                            class="absolute w-3/5 h-full z-10 p-1 -translate-y-1/2 top-1/2 right-3 rounded-3xl bg-white dark:bg-body shadow-lg shadow-box-shadow border border-box-border">
                            <img src="/images/owndays-hero-banner.png" alt="In studio" width="500" height="auto" loading="lazy"
                                class="w-full h-full rounded-2xl object-cover">
                        </div>
                        <div
                            class="absolute  -translate-y-1/2 top-1/2 h-[calc(80%-2rem)] w-[calc(40%-20px)] p-1 rounded-3xl bg-white dark:bg-body shadow-lg shadow-box-shadow border border-box-border ">
                            <img src="/images/owndays-hero-banner2.webp" alt="Happy in studio" width="200" height="auto"
                                loading="lazy" class="w-full h-full rounded-2xl object-cover">
                        </div>
                    </div>
                </div>
            </div>
        </AtomsContainer>
    </section>
</template>