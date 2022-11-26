<template>
    <div class="energy py-4">
        <h2><span>They already made the decison</span> to not waste anymore energy</h2>
        <div class="container">
            <div class="row mt-5">
                <div class="col-lg-4 col-md-6 col-sm-12" v-for="c in 3">
                    <div class="shadow py-4 px-2 parent">
                        <img v-if="c == 1" src="@/assets/quote-face-man.svg" alt="" class="w-25">
                        <img v-else-if="c == 2" src="@/assets/quote-face-woman.svg" alt="" class="w-25">
                        <img v-else src="@/assets/quote-face-man-beard.svg" alt="" class="w-25">
                        <p class="a" v-if="c == 1">Michel</p>
                        <p class="a" v-else-if="c == 2">Laura</p>
                        <p class="a" v-else>Jérôme</p>
                        <span v-for="a in 4">
                            <span><svg data-v-ef4bc576="" data-v-fde73a0c="" height="27" width="27" viewBox="0 0 27 27"
                                    class="vue-star-rating-star" step="50">
                                    <linearGradient data-v-ef4bc576="" id="2kth0v" x1="0" x2="100%" y1="0" y2="0">
                                        <stop data-v-ef4bc576="" offset="100%" stop-color="#FBB829" stop-opacity="1">
                                        </stop>
                                        <stop data-v-ef4bc576="" offset="100%" stop-color="#d8d8d8" stop-opacity="1">
                                        </stop>
                                    </linearGradient>
                                    <filter data-v-ef4bc576="" id="vumbc7" height="130%" width="130%"
                                        filterUnits="userSpaceOnUse">
                                        <feGaussianBlur data-v-ef4bc576="" stdDeviation="0" result="coloredBlur">
                                        </feGaussianBlur>
                                        <feMerge data-v-ef4bc576="">
                                            <feMergeNode data-v-ef4bc576="" in="coloredBlur"></feMergeNode>
                                            <feMergeNode data-v-ef4bc576="" in="SourceGraphic"></feMergeNode>
                                        </feMerge>
                                    </filter>
                                    <!---->
                                    <polygon data-v-ef4bc576=""
                                        points="12.272727272727272,1.3636363636363635,4.09090909090909,27,24.545454545454543,10.636363636363635,0,10.636363636363635,20.454545454545453,27"
                                        fill="url(#2kth0v)" stroke="#999" stroke-width="0" stroke-linejoin="miter">
                                    </polygon>
                                    <polygon data-v-ef4bc576=""
                                        points="12.272727272727272,1.3636363636363635,4.09090909090909,27,24.545454545454543,10.636363636363635,0,10.636363636363635,20.454545454545453,27"
                                        fill="url(#2kth0v)"></polygon>
                                </svg></span>
                        </span>
                        <span>
                            <svg data-v-ef4bc576="" data-v-fde73a0c="" height="27" width="27" viewBox="0 0 27 27"
                                class="vue-star-rating-star" step="50">
                                <linearGradient data-v-ef4bc576="" id="91z4" x1="0" x2="100%" y1="0" y2="0">
                                    <stop data-v-ef4bc576="" offset="50%" stop-color="#FBB829" stop-opacity="1"></stop>
                                    <stop data-v-ef4bc576="" offset="50%" stop-color="#d8d8d8" stop-opacity="1"></stop>
                                </linearGradient>
                                <filter data-v-ef4bc576="" id="1z0bef" height="130%" width="130%"
                                    filterUnits="userSpaceOnUse">
                                    <feGaussianBlur data-v-ef4bc576="" stdDeviation="0" result="coloredBlur">
                                    </feGaussianBlur>
                                    <feMerge data-v-ef4bc576="">
                                        <feMergeNode data-v-ef4bc576="" in="coloredBlur"></feMergeNode>
                                        <feMergeNode data-v-ef4bc576="" in="SourceGraphic"></feMergeNode>
                                    </feMerge>
                                </filter>
                                <!---->
                                <polygon data-v-ef4bc576=""
                                    points="12.272727272727272,1.3636363636363635,4.09090909090909,27,24.545454545454543,10.636363636363635,0,10.636363636363635,20.454545454545453,27"
                                    fill="url(#91z4)" stroke="#999" stroke-width="0" stroke-linejoin="miter"></polygon>
                                <polygon data-v-ef4bc576=""
                                    points="12.272727272727272,1.3636363636363635,4.09090909090909,27,24.545454545454543,10.636363636363635,0,10.636363636363635,20.454545454545453,27"
                                    fill="url(#91z4)"></polygon>
                            </svg>
                        </span>
                        <p v-if="c == 1" class="mt-3 c">Nice App, very good thermostat and a responsive support team.
                            Since the first month, I can see real energy savings done.</p>
                        <p v-else-if="c == 2" class="mt-3 c">An efficient thermostat, a very comprehensive support team
                            and regular updates! It is rare to see such service these days.</p>
                        <p v-else class="mt-3 c">Efficient and simple App, very satisfying product. Thank you for making
                            our life easier.</p>
                        <i class="fa-solid fa-quote-right"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="saving_money mt-5 py2">
        <h2><span>Start saving</span> money and energy</h2>
        <div class="shadow ex py-4 pare">
            <img src="@/assets/product-essential-thumbnail.png" class="img-fluid image" alt="rabbit">
            <div class="container">
                <h2>Ween Pack</h2>
                <p id="paragrabh">From 159$</p>
                <div>
                    <ul class="checkmark">
                        <li><i class="fa-solid fa-check"></i>Ween thermostat and relay </li>
                        <li><i class="fa-solid fa-check"></i>Free delivery</li>
                        <li><i class="fa-solid fa-check"></i>2 year warranty</li>
                        <li><i class="fa-solid fa-check"></i>Available technical support</li>
                        <li><i class="fa-solid fa-check"></i>Cloud hosted in France</li>
                    </ul>

                    <p class="text-center mt-5 f py-2"><b>Save 10$</b>choosing to receive your Ween Pack with a reduced
                        and low carbon footprint
                        packaging</p>
                    <button class="btns btn py-2">Buy 159$</button>
                    <p class="py-2 text-center">Or receive your Ween Pack in its classic packaging.</p>
                    <button class="btn py-2">Buy 169$</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
        }
    }
}
</script>

<style scoped>
h2 {
    font-weight: 700;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    text-align: center;
}

span {
    color: #36c89b;
}

.energy {
    margin-top: 100px;
}



b {
    color: #264057;
}
.parent{
    position:relative;
}
.a {
    font-weight: 700;
    font-size: 25px;
    color: #264057;
    letter-spacing: 1px;
    margin-left: 10px;
}

.f {
    font-weight: 400;
}

.c {
    width: 70%;
    color: #264057;
    font-weight: 500;
    font-style: italic;
    min-height: 90px;
}



.fa-quote-right{
    position: absolute;
    background-color: #36c89b;
    color: white;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    right: 10px;
    bottom: 10px;
}
.fa-check{
    background-color:#36c89b;
    width:23px;
    height:23px;
    display: inline-block;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    margin-right:5px;
    text-align: center;
    padding-top: 2px;
    color:white;
}
.btns {
    background-color: #36c89b;
    color: white;
    border-radius: 50px;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.btns:hover {
    opacity: 0.8;
}

.btn {
    border: 1px solid #9afddf;
    border-radius: 50px;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.btn:hover {
    border: 1px solid #36c89b;
    transition: 0.3s ease all;
}

ul {
    list-style-type: none;
    text-align: left;
}

ul li {
    padding:10px;
    border-bottom: 1px solid rgb(247, 237, 237)
}


.ex {
    width: 22%;
    text-align: center;
    margin: 120px auto;
    background-color: white;
    position: relative;
}

h2 {
    color: #264057;
}

#paragrabh {
    color: #36c89b;
    font-weight: 700;
    font-size: 18px;
}

.container {
    margin-top: 100px;
}

.image {
    position: absolute;
    top: -15%;
    left: -1%;
}

@media(max-width: 768px){
    .pare{
        width:90%;
    }
}



</style>