<template>
<div class="swiper">
  <div class="swiper-container" id="swiperOne">
    <div class="swiper-wrapper">
      <div class="swiper-slide" v-for="(item,index) in img" :key="index">
         <img :src="item.pic" />
      </div>
    </div>
         <img  class="swiper-button-prev" id="one" src="../../assets/imgs/首页改1_10.gif" alt="">
         <img class="swiper-button-next" id="two" src="../../assets/imgs/首页改1_13.gif" alt="">
    <!-- 如果需要分页器 -->
    <div class="swiper-pagination nc">
    </div>

  </div>
  </div>
</template>
<script>
//引入swiper
import Swiper from "swiper";
import "swiper/css/swiper.css";

export default {
  data: function () {
    return {
        img:[
            {pic:require("../../assets/imgs/首页改1_27.gif")},
            {pic:require("../../assets/imgs/首页改1_68.gif")},
            {pic:require("../../assets/imgs/首页改1_71.gif")},
            {pic:require("../../assets/imgs/首页改1_72.gif")},
            {pic:require("../../assets/imgs/首页改1_75.gif")},
            {pic:require("../../assets/imgs/首页改1_71.gif")}
        ]
    };
  },
  async mounted() {
    var mySwiper = new Swiper("#swiperOne", {
      loop: true, // 循环模式选项
      autoplay: {
        disableOnInteraction: false,
        delay:2000,
      },
      // 如果需要分页器
      pagination: {
        el: ".swiper-pagination",
      },
      navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
    })
  },
};
</script>
<style scoped>
.swiper{
    position: relative;
    width: 3.75rem;
    height: 1.50rem;
}

.swiper-slide img{
    width: 3.75rem;
    height: 1.50rem;
}
#one{
    position: absolute;
    width: .32rem;
   	height: .31rem;
    top: 50%;
    left: .20rem;
}
#one1{
    display: none;
}
#one :hover+#one1{
    display: inline-block;
    z-index: 100;
    
}
/* #one1{
    position: absolute;
    width: .32rem;
	height: .31rem;
    top: 80%;
    left: .20rem;
    display: inline-block;
}
#one:hover #one1{
    display: block;
    border: 3px solid red;
} */
#two{
   position: absolute;
    width: .32rem;
  	height: .31rem;
    right: .20rem;
    left: 3.2rem;
    opacity: 0.5;
    top: 50%;
    z-index: 999;
    
}
.swiper-pagination-bullet swiper-pagination-bullet-active{
	width: .07rem;
	height: .07rem;
	background-color: #00f0ff;
}
</style>