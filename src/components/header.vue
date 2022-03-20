<template>
    <div id="d1">
        <header id="d2">
            <a href="http://www.baidu.com"></a>
            <ul class="top_list">
                <li v-for="(item,k) of arr1" :key="k" :class="{top_list_active:k==0}">{{item}}</li>
            </ul>
            <div class="input"><i></i><input type="text" placeholder="音乐/电台/用户"></div>
            <div class="video"><div>视频投稿</div></div>
            <div class="login"><span>登陆</span><i></i>
                <ul class="login_list">
                    <li><i></i><span>手机号登陆</span></li>
                    <li><i></i><span>微信登陆</span></li>
                    <li><i></i><span>qq号登陆</span></li>
                    <li><i></i><span>新浪微博登陆</span></li>
                    <li><i></i><span>网易邮箱登陆</span></li>
                </ul>
            </div>
        </header>
        <!-- <section>
            <swiper :options="swiperOption">
                <swiper-slide>于</swiper-slide>
                <swiper-slide>立</swiper-slide>
                <swiper-slide>伟</swiper-slide>
                <swiper-slide>很</swiper-slide>
                <swiper-slide>帅</swiper-slide>
                <swiper-slide>是</swiper-slide>
                <swiper-slide>真</swiper-slide>
                <swiper-slide>的</swiper-slide>
            </swiper>
        </section> -->
    </div>
</template>
<script>
    export default{
        name:"HeaderVue",
        data(){
            return {
                arr1:["发现音乐","我的音乐","朋友","商城","音乐人","下载客户端"],
                swiperOption:{
                    
                }
            }
        },
        methods:{
        },
        created(){
            console.log(this.msg)
        },
    }
</script>
<style scoped>
.c1{
    color:#fff;
    text-shadow: 2px 2px #fff;
}
    #d1{
        background: #232323;
    }
    #d2{
        margin:0 auto;
        width:1200px;
        height:70px;
        display:flex;
        justify-content: space-between;
        align-items: center;
    }
    #d2>a{
        width:176px;
        height:70px;
        background:url(../assets/topbar.png) no-repeat;
    }
    .top_list>li{
        float:left;
        padding: 0 19px;
        font-size: 1em;
        height:70px;
        line-height: 70px;
        color:#AAA;
        cursor:pointer;
        transition: all 0.3s linear;
    }
    .top_list>li:hover,li.top_list_active{
        color:white;
        background:#000;
    }
    .input{
        width: 158px;
        height: 32px;
        border-radius: 16px;
        background-color: #fff;
        margin-left:28px;
        display:flex;
        justify-content: flex-start;
        align-items: center;
    }
    .input>i{
        display:inline-block;
        width:33px;
        height:33px;
        background:url(../assets/topbar.png) no-repeat;
        background-position:0 -99px;
    }
    .input>input{
        font-size: 0.8em;
        background-color: transparent;
        width: 100px;
        vertical-align: sub;
        border: none;
        outline: none;
    }
    .video{
        width: 90px;
        height: 100%;
        overflow: hidden;
    }
    .video>div{
        background-position: 0 -140px;
        margin-top: 20%;
        width: 100%;
        height: 32px;
        border-radius: 16px;
        line-height: 31px;
        font-size: 0.8em;
        color: #ccc;
         background:url(../assets/topbar.png) no-repeat;
        background-position:0 -140px;
        padding-left:31px;
    }
    .video>div:hover{
        background-position:-100px -140px;
        color:#fff;
    }
    .login{
        width: 48px;
        font-size: 0.9em;
        line-height: 70px;
        background-position: right -27px;
        position: relative;
        color: #bbb;
    }
    .login>i{
        background:url(../assets/toplist.png) no-repeat;
        display:inline-block;
        background-position:-20px 0;
        width:14px;
        height:8px;
        transform:rotate(180deg);
    }
    .login_list{
        position:absolute;
        top:58px;
        left:-70px;
        z-index:100;
        border-radius: 5px;
        overflow: hidden;
        transform:scaleY(0);
        transform-origin: center 0 0;
        transition: transform 0.3s ease, opacity 0.3s ease;
    }
    .login_list>li{
        width:168px;
        height:39px;
        display:flex;
        justify-content: flex-start;
        align-items: center;
        color:#bbb;
        background-color:#2A2A2A;
        font-size:1em;
        cursor: pointer;
    }
    .login_list>li>i{
        background:url(../assets/toplist.png) no-repeat;
        background-position: 0 0;
        display:inline-block;
        width: 18px;
        height: 18px;
        margin-left: 19px;
        margin-right: 5px;
        vertical-align: middle;
    }
    .login_list>li:nth-child(2)>i{
        background-position: -20px -20px;
    }
    .login_list>li:nth-child(3)>i{
        background-position: -20px -40px;
    }
    .login_list>li:nth-child(4)>i{
        background-position: 0px -20px;
    }
    .login_list>li:nth-child(5)>i{
        background-position: 0px -40px;
    }
    .login_list>li>span{
        display:inline-block;
        height:100%;
        line-height: 39px;
        text-align: left;
        
    }
    .login:hover>.login_list{
        transform:scaleY(1);
    }
</style>