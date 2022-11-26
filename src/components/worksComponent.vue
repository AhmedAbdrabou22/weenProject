<template>
    <div class="works py-4">
        <div>
            <a href="#">
                <img src="https://www.ween.fr/img/bunney-nose.svg" alt="MouseHover">
            </a>
        </div>
        <div class="text-center mt-5 revolutionises  py-5">
            <div class="d m-auto">
                <h1><span>How</span> it works?</h1>
                <p class="mt-5 py-4 par">The Ween thermostat <b>revolutionises programming your heating</b> based your
                    daily
                    routine and location.
                    It detects when you leave and anticipates your return to adjust the temperature perfectly.
                    All without any input from you. <span>Magic!</span></p>
            </div>
            <div class="mt-5 homeImage">
                <img src="@/assets/ween-how-it-works.svg" alt="">
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
.works {
    margin-top: 120px;
}

.works a {
    position: relative;
    display: block;
    width: 25px;
    margin: auto;
    animation: example 0.5s infinite alternate;
    transition: 0.2s all ease;
}

.d {
    width: 50%;
}

@keyframes example {
    0% {
        top: 15px
    }

    100% {
        top: 0px
    }
}

.revolutionises h1 {
    color: #264057;
    font-weight: 700;
}

.revolutionises p {
    font-weight: 400;
}

.revolutionises span {
    color: #74f1cb;
}

.homeImage img {
    width: 80%;
}

@media(max-width:768px) {
    .d {
        width: 100%;
    }
}
</style>