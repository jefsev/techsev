<template>
    <div id="pageHero">
        <div class="hero-content flex flex-col justify-center">
            <div class="hero-inner flex flex-row justify-between items-start">
                <div class="title">
                    <h1>HI THERE!</h1>
                </div>
                <div class="intro">
                    <p>
                        My name is Jeffrey Sevinga. I’m a developer from the
                        Netherlands.
                    </p>
                    <span class="text-link"
                        >Let’s talk:
                        <a href="https://wa.me/031682516209">WhatsApp</a> or
                        <a href="mailto:sevinga@protonmail.com">Mail</a>
                    </span>
                </div>
            </div>
        </div>
        <div class="hero-footer flex flex-col items-center">
            <div class="hero-what flex flex-row justify-center items-center">
                <span>DEVELOPER</span>
                <span class="dot">.</span>
                <span>COFFEE</span>
            </div>
            <a href="#" v-scroll-to="'#about'">
                <img src="/scroll.svg" alt="" />
            </a>
        </div>
    </div>
</template>
