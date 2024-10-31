<template>
    <footer class="pt-20 bg-zinc-100 dark:bg-body border-t border-zinc-200 dark:border-zinc-100/20">
        <AtomsContainer class-name="pb-10">
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 gap-y-10">
                <div class="col-span-2 md:col-span-4 lg:col-span-2">
                    <NuxtLink to="/" class=" flex items-center gap-2">
                        <span class="flex">
                            <img :src="logoSrc" width="40" alt="logo" class="w-fit h-min object-cover">
                        </span>
                    </NuxtLink>
                    <p class="text-primary dark:text-zinc-400 pt-6">
                        At OWNDAYS Labs, we blend cutting-edge technology with exceptional design to bring you eyewear that enhances both your style and vision. Discover innovation and quality with each pair.
                    </p>
                </div>
                <BlocksFooterNavBlock title="Shop" :links="shopLinks" />
                <BlocksFooterNavBlock title="Purchase Information" :links="purchaseLinks" />
                <BlocksFooterNavBlock title="About OWNDAYS" :links="aboutLinks" />
                <BlocksFooterNavBlock title="Support" :links="supportLinks" />
            </div>
        </AtomsContainer>
        <div class="py-2 bg-zinc-200 dark:bg-primary">
            <AtomsContainer>
                <div class="flex justify-center items-center gap-5 text-primary dark:text-zinc-400">
                    <div class="">
                        &copy; {{ new Date().getFullYear() }} Allright Reserved. Designed by <NuxtLink target="_blank"
                            to="#" class="font-bold text-primary dark:text-secondary">Surakiat Tablakorn</NuxtLink>
                    </div>
                </div>
            </AtomsContainer>
        </div>
    </footer>
</template>

<script lang="ts" setup>
const shopLinks = [
    { href: "#", text: "Eyeglasses" },
    { href: "#", text: "Sunglasses" },
    { href: "#", text: "All Brands" },
    { href: "#", text: "Special Offers" }
];

const purchaseLinks = [
    { href: "#", text: "Our Lenses" },
    { href: "#", text: "OWNDAYS Customer Guarantees" },
    { href: "#", text: "International Shipping Service" }
];

const aboutLinks = [
    { href: "#", text: "All Stores" },
    { href: "#", text: "All Services" },
    { href: "#", text: "Lens Replacement Service" },
    { href: "#", text: "OWNDAYS Membership" },
    { href: "#", text: "Company Info" },
    { href: "#", text: "Careers" },
    { href: "#", text: "Eye Camp" }
];

const supportLinks = [
    { href: "#", text: "FAQs" },
    { href: "#", text: "Website Usage Guide" },
    { href: "#", text: "Sitemap" },
    { href: "#", text: "New Customer Guide" },
    { href: "#", text: "Create New Account" }
];

const logoSrc = ref('/logo-owndays-white.png');

onMounted(() => {
    const updateLogoSrc = () => {
        logoSrc.value = document.documentElement.classList.contains('dark')
            ? '/logo-owndays-white.svg'
            : '/logo-owndays-dark.svg';
    };

    updateLogoSrc();

    const observer = new MutationObserver(updateLogoSrc);
    observer.observe(document.documentElement, { attributes: true, attributeFilter: ['class'] });

    onUnmounted(() => {
        observer.disconnect();
    });
});

</script>