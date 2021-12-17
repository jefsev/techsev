<template>
    <div class="container">
        <TheHeader />
        <PageHero />

        <div id="pageBody">
            <div class="illustration">
                <img src="/illustration.svg" alt="" />
            </div>
            <div class="content container-small">
                <nuxt-content :document="page" />
            </div>
        </div>

        <TheFooter />
    </div>
</template>

<script>
export default {
    name: "IndexPage",
    async asyncData({ $content }) {
        const page = await $content("home").fetch();

        return {
            page,
        };
    },
};
</script>
