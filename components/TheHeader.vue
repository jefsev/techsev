<template>
    <div id="nav" class="flex flex-row justify-between items-center">
        <span class="menu-logo">TECHSEV<span>.</span></span>

        <nav class="navbar flex flex-row justify-end items-center">
            <a href="#" v-scroll-to="'#about'">about me</a>
            <a href="#" v-scroll-to="'#works'">works</a>
            <div class="contact flex flex-row justify-end items-center">
                <a href="https://github.com/jefsev" target="_blank">
                    <img src="/github.svg" alt="" />
                </a>
                <a href="mailto:sevinga@protonmail.com" target="_blank">
                    <img src="/email.svg" alt="" />
                </a>
                <a href="https://wa.me/031682516209" target="_blank">
                    <img src="/whatsapp.svg" alt="" />
                </a>
            </div>
        </nav>
    </div>
</template>

