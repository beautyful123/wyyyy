<!--

    swiper轮播

-->
<template lang="">
    <div class="wrap">
        <div class="swiperBox" @mouseenter="mousein" @mouseleave="mouseout">
            <!-- img -->
            <div class="imgBox" ref="swiper" :style="{transform:rot}">
                <img src="../assets/banner/banner1.png" alt="">
                <img src="../assets/banner/banner2.png" alt="">
                <img src="../assets/banner/banner3.png" alt="">
                <img src="../assets/banner/banner4.png" alt="">
                <img src="../assets/banner/banner5.png" alt="">
                <img src="../assets/banner/banner6.png" alt="">
                <img src="../assets/banner/banner7.png" alt="">
                <img src="../assets/banner/banner8.png" alt="">
            </div>
            <!-- btn -->
            <ul class="btnBox">
                <li @click="prev"> < </li>
                <li @click="next"> > </li>
            </ul>
            <ul class="paginations">
                <li @click="toggle(0)" :style="{boxShadow:Math.abs(reg%360)==0?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(45)" :style="{boxShadow:Math.abs(reg%360)==45?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(90)" :style="{boxShadow:Math.abs(reg%360)==90?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(135)" :style="{boxShadow:Math.abs(reg%360)==135?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(180)" :style="{boxShadow:Math.abs(reg%360)==180?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(225)" :style="{boxShadow:Math.abs(reg%360)==225?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(270)" :style="{boxShadow:Math.abs(reg%360)==270?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
                <li @click="toggle(315)" :style="{boxShadow:Math.abs(reg%360)==315?'0 0 10px rgba(255, 80, 90, 1)':' 0 0 10px rgba(255, 255, 255, 0.5)'}"></li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name:"HomeSwiper",
    data(){
        return{
            reg:0,
            clock:"",
        }
    },
    computed:{
        rot(){
            return `rotateY(${this.reg}deg)`;
        }
    },
    methods:{
        prev(){
            this.reg+=45;
        },
        next(){
            this.reg-=45;
        },
        mousein(){
            clearInterval(this.clock);
        },
        mouseout(){
            this.clock = setInterval(() => {
                this.reg-=45;
            },3000)
        },
        toggle(n){
            this.reg = -n;
        }
       
    },
    mounted(){
        this.clock = setInterval(() => {
            this.reg-=45;
        },3000)
    }
}
</script>
<style scoped>
    *{
        margin: 0;
        padding:0;
        box-sizing: border-box;
    }
    .wrap{
        width:100%;
        height:370px;
        background-image: linear-gradient(60deg, #29323c 0%, #485563 100%);
        overflow: hidden;
    }
    .swiperBox{
        position:relative;
        margin:0 auto;
        width:1200px;
        height: 100%;
        /* 视距500px */
        perspective: 500px;
        overflow: hidden;
    }
    .imgBox{
        position:relative;
        margin:11px auto 0;
        width:730px;
        height: 336px;
        transform-style: preserve-3d;
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transition: transform .5s;
    }
    .imgBox img{
        backface-visibility: hidden;
        -webkit-backface-visibility: hidden;
        position:absolute;
        left:0;
        top:0;
        box-shadow: 0px 8px 70px rgba(0, 0, 0, 1);
    }
    .imgBox>img:nth-child(2){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(45deg);
    }
    .imgBox>img:nth-child(3){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(90deg);
    }
    .imgBox>img:nth-child(4){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(135deg);
    }
    .imgBox>img:nth-child(5){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(180deg);
    }
    .imgBox>img:nth-child(6){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(225deg);
    }
    .imgBox>img:nth-child(7){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(270deg);
    }
    .imgBox>img:nth-child(8){
        transform-origin: center center -881.188px;
        -webkit-transform-origin: center center -881.188px;
        transform: rotateY(315deg);
    }
    /* btnBox */
    .btnBox>li:first-child{
        position:absolute;
        top:calc(50% - 41px);
        left:-48px;
        width:48px;
        height: 82px;
        font-size:50px;
        color:white;
        transition:all .5s;
        text-align:center;
        line-height: 82px;
        font-family:kaiti;
        cursor: pointer;
    }
    .btnBox>li:last-child{
        position:absolute;
        top:calc(50% - 41px);
        right: -48px;
        width:48px;
        height: 82px;
        font-size:50px;
        color:white;
        transition:all .5s;
        text-align:center;
        line-height: 82px;
        font-family:kaiti;
        cursor: pointer;
    }
    .btnBox>li:hover{
        background:rgba(0,0,0,.2);
    }
    .swiperBox:hover li:first-child{
        left:10px;
    }
    .swiperBox:hover li:last-child{
        right:10px;
    }
    .paginations{
        margin:3 auto;
        display:flex;
        justify-content: center;
        align-items: center;
    }
    .paginations li{
        margin:5px 12px;
        border-radius: 50%;
        width:10px;
        height:10px;
        box-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
        cursor: pointer;
        /* box-shadow: 0 0 10px rgba(255, 80, 90, 1); */
    }
</style>