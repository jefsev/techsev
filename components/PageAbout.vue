<template>
    <div id="pageBody">
        <div class="illustration">
            <img src="/illustration.svg" alt="" />
        </div>
        <div class="content container-small">
            <div class="about">
                <nuxt-content :document="about" />
            </div>
            <div class="tools"></div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return { about: {} };
    },
    async fetch() {
        this.about = await this.$content("about").fetch();
    },
};
</script>

