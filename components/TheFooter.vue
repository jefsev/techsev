<template>
    <div id="footer">
        <div class="footer-contact flex justify-center">
            <a
                href="https://www.linkedin.com/in/jeffrey-sevinga-46852a11b/"
                target="_blank"
                >LINKEDIN</a
            >
            <a href="mailto:sevinga@protonmail.com" target="_blank">EMAIL</a>
            <a href="https://wa.me/031682516209" target="_blank">WHATSAPP</a>
            <a href="https://github.com/jefsev" target="_blank">GITHUB</a>
        </div>
        <div class="footer-foot flex justify-between items-center">
            <div class="foot-left">
                <span
                    >© {{ currentDate.getFullYear() }}
                    <span class="logo">TECHSEV<span class="dot">.</span></span>
                </span>
            </div>
            <span class="dot absolute">.</span>
            <div class="foot-right">
                <span>0% COOKIES</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            currentDate: new Date(),
        };
    },
};
</script>

