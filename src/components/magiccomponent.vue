<template>
    <div class="magic">
        <h2><span>Discover</span> the magic world of Ween</h2>
        <div class="circlInfo">
            <div class="imagecont">
                <div class="actImage" ref="imagecont">
                    <img src="@/assets/ecosystem-thermostat.png" alt="Tghermostat">
                    <span>Smart thermostat</span>
                </div>
                <i class="fa-solid fa-plus  c" @click="run"></i>
            </div>
            <!--System-->
            <div class="conta">
                <div class="actImage" ref="conta">
                    <img src="@/assets/ecosystem-app.png" alt="ecosystem" class="img-fluid">
                    <span>APP</span>
                </div>
                <i class="fa-solid fa-plus  s" @click="run"></i>
            </div>
            <div class="contatwo">
                <div class="actImage" ref="conta">
                    <img src="@/assets/ecosystem-relay.png" alt="ecosystem" class="img-fluid">
                    <span class="mx-2">Relay</span>
                </div>
                <i class="fa-solid fa-plus  d" @click="run"></i>
            </div>
            <div class="letter text-left">
                <p v-if="c">
                    <b>Smart thermostat</b> <br> The hardware optimises and allows you to customise the temperature of your home,
                    based on location and daily routine. Delivering a tailored hearing experience.</p>
                    <p v-if="s">
                        <b>APP</b><br>
                        Your thermostat and the App communicate and work together to best adapt your home temperature. Via the App, you can adjust in real-time your settings and check your savings.</p>
                    <p v-if="d"><b>Relay</b> <br/>
                        The relay is aptly as it connects any type of heating system to the Ween thermostat. All done wirelessly, of course.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            c: false,
            s:false,
            d:false,
        }
    },
    mounted() {
        let fa_solids = document.querySelectorAll('.fa-plus');
        fa_solids.forEach((ele => {
            ele.addEventListener('click', () => {
                fa_solids.forEach(ele => {
                    ele.previousElementSibling.classList.remove('styleopa')
                    ele.classList.remove('fa-sharp', 'fa-solid', 'fa-xmark')
                    ele.classList.add('fa-solid', "fa-plus")
                    ele.style.backgroundColor = "#36c89b"
                })
                ele.previousElementSibling.classList.add('styleopa')
                ele.classList.remove('fa-solid', "fa-plus")
                ele.classList.add('fa-sharp', 'fa-solid', 'fa-xmark')
                ele.style.backgroundColor = "#264057"
                if(ele.classList.contains('d')){
                    this.d = true;
                    this.s = false;
                    this.c=false;
                }else if(ele.classList.contains('s')){
                    this.s = true;
                    this.d = false;
                    this.c = false;
                }else{
                    this.c = true;
                    this.d = false;
                    this.s = false;
                }
            })
        }))
        console.log(this.$refs.imagecont);
    },
    methods: {

    }
}
</script>

<style scoped>
h2 {
    text-align: center;
}

span {
    color: #36c89b;
}

.styleopa {
    opacity: 0.7;
}

.circlInfo {
    margin: 120px auto;
    width: 600px;
    height: 600px;
    border-radius: 50%;
    border: 2px solid #36c89b;
    position: relative;
}

.letter {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color:#264057;
    font-weight: 600;
}

.circlInfo .imagecont {
    position: absolute;
    top: -80px;
    left: 35%;
}

.circlInfo .conta {
    position: absolute;
    top: 60%;
    left: -10%;
}

.circlInfo .contatwo {
    position: absolute;
    top: 60%;
    right:-40%;
}

.circlInfo .imagecont .actImage img,
.circlInfo .conta .actImage img,
.circlInfo .contatwo .actImage img {
    width: 35%;
}

.circlInfo .imagecont .actImage span,
.circlInfo .conta .actImage span,
.circlInfo .contatwo .actImage span {
    color: #264057;
    vertical-align: top;
    font-weight: 700;
    font-size: 25px;
}

.circlInfo .conta .actImage span {
    vertical-align: middle;
}

.fa-solid {
    background-color: #36c89b;
    width: 40px;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    margin-right: 5px;
    text-align: center;
    padding-top: 2px;
    color: white;
    cursor: pointer;
}

.conta {
    position: relative;
}

.conta .fa-solid {
    position: absolute;
    right: 200px;
    top: 65%;
    cursor: pointer;
}

@media(max-width: 768px){
    .circlInfo {
    width: 300px;
    height: 300px;
    margin:100px auto;
}
.circlInfo .imagecont .actImage img,
.circlInfo .conta .actImage img,
.circlInfo .contatwo .actImage img {
    width: 40%;
}
.circlInfo .imagecont .actImage span,
.circlInfo .conta .actImage span,
.circlInfo .contatwo .actImage span{
    display: none;
}
.fa-solid {
    background-color: #36c89b;
    width: 20px;
    height: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    margin-right: 5px;
    text-align: center;
    padding-top: 2px;
    color: white;
    cursor: pointer;
}
.letter{
    font-size: 14px;
    width:70%;
    z-index: -1;
}
}
</style>