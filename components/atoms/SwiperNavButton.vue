<template>
    <button class="outline-none p-3 rounded-full relative group text-zinc-700 dark:text-zinc-400 bg-body">
        <span class="absolute inset-0 rounded-full group-hover:scale-105 origin-center transition-all ease-in-out border border-box-border border-zinc-300"></span>
        <span class="relative">
            <slot/>
        </span>
    </button>
</template>