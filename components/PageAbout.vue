<template>
    <div id="pageBody">
        <div class="illustration">
            <img src="/illustration.svg" alt="" />
        </div>
        <div class="content container-small" id="about">
            <div class="about">
                <nuxt-content :document="about" />
            </div>
            <div class="tools">
                <nuxt-content :document="tools" />
            </div>
        </div>
        <div class="quote-block">
            <span
                >“Make it simple, but significant.”
                <span class="yel">—</span> Don Draper</span
            >
        </div>
        <div class="content container-small" id="works">
            <nuxt-content :document="works" />
            <div
                class="
                    works-logos
                    flex flex-row flex-wrap
                    justify-between
                    items-center
                "
            >
                <a href="https://bijbelseoverdenkingen.nl/" target="_blank">
                    <img src="/logo-whitetext.svg" />
                </a>
                <a href="https://events.lekkerboats.com/" target="_blank">
                    <img src="/lekkerwhite.svg" />
                </a>
                <a href="https://vbstaircases.com/" target="_blank">
                    <img src="/logo-bruchen.svg" />
                </a>
                <a href="https://108tattoostudio.nl/" target="_blank">
                    <img src="/108.svg" />
                </a>
                <a href="https://sevinga-stoffering.nl/" target="_blank">
                    <img src="/Sevingastoffering-logo.svg" />
                </a>
                <a
                    href="https://www.brandsmaverzekeringen.com/"
                    target="_blank"
                >
                    <img src="/brandsma.svg" />
                </a>
                <a href="https://www.rondomspraak.nl/" target="_blank">
                    <img src="/rondom.svg" />
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            about: {},
            tools: {},
            works: {},
        };
    },
    async fetch() {
        this.about = await this.$content("about").fetch();
        this.tools = await this.$content("toolsandskills").fetch();
        this.works = await this.$content("works").fetch();
    },
};
</script>

