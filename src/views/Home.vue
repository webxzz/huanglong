<template>
    <div class="wrap">
          <header class="header">
              <div class="header_top">
                <p>欢迎来到紧缺应用技术技能型人才职业教育报考平台</p>
              </div>
              <Yuicon/>
              <Lunbo/>
          </header>
          <main class="main">
            <Title />
            
          </main>
          <footer class="footer">
            <!-- <div class="footer_top"> -->
              <div class="footer_a">
                   <p>
                     <span>
                        <svg class="icon" aria-hidden="true">
                            <use xlink:href="#icon-dianhua"></use>
                        </svg>
                     </span>
                     <span>电话咨询</span>
                   </p>
              </div>
               <div class="footer_b">
                  <p>
                     <span>
                        <svg class="icon" aria-hidden="true">
                            <use xlink:href="#icon-kefu"></use>
                        </svg>
                     </span>
                     <span>在线咨询</span>
                   </p>
              </div>
               <div class="footer_c">
                   <p>
                     <span>
                        <svg class="icon" aria-hidden="true">
                            <use xlink:href="#icon-renyuanbaoming"></use>
                        </svg>
                     </span>
                     <span>在线报名</span>
                   </p>
              <!-- </div> -->
             </div> 
          </footer>
    </div>
</template>

<script>
import Yuicon from '@/views/yuicon'
import Lunbo from '@/views/lunbo/lunbo.vue'
import Title from '@/views/title'

  export default {
    components: {
        Yuicon,
        Lunbo,
        Title
     },
      data(){
        return{
        
        }
      }
  }
</script>

<style lang="scss" scoped>
.icon {
      width: 0.20rem; height: 0.19rem;
      vertical-align: -0.15em;
      fill: currentColor;
      overflow: hidden;
  }
input{
  background:none;  
	outline:none;  
	border:none;
}
.wrap{
  // height: 100%;
  display: flex;
  flex-direction: column;
  .header{
      width: 3.75rem;
      margin: 0 auto;
      .header_top{
        width: 3.75rem;
        height: 0.3rem;
        background: #fff;
        // display: flex;
        // align-items: center;
        p{
          // width: 2.80rem;
          height: 0.3rem;
          font-family: PingFang-SC-Medium;
          font-size: 0.12rem;
          font-weight: normal;
          font-stretch: normal;
          letter-spacing: 0rem;
          color: #777777;
          margin: 0 0 0 0.13rem;
          line-height: 0.3rem;
        }
      }
  }
  .main{
     flex: 1; 
     overflow-y: scroll;
  }
  .footer{
    width: 100%;
    height: 0.42rem;
    background: #eaeaea;
      display: flex;
     justify-content: space-around;
    // .footer_top{
    //   width: 3.75rem;
    //   margin: 0 auto;
    //   display: flex;
    //  justify-content: space-around;
      .footer_a{
        width: 1.22rem;
        height: 0.42rem;
        background-color: #1776af;
        border-radius: 0.06rem 0.06rem 0rem;
        p{
        line-height: 0.42rem;
        text-align: center;
          span:nth-child(1){
            color: #ffffff;
            margin: 0 0.08rem;
            position: relative;
            top: 0.04rem;
          }
          span:nth-child(2){
              font-size: 0.13rem;
              color: #ffffff;
          }
        }
      }
      .footer_b{
        width: 1.24rem;
        height: 0.42rem;
        background-color: #1776af;
        border-radius: 0.06rem 0.06rem 0 0;
        p{
          line-height: 0.42rem;
          text-align: center;
            span:nth-child(1){
              color: #ffffff;
              margin: 0 0.08rem;
              position: relative;
              top: 0.04rem;
            }
            span:nth-child(2){
                font-size: 0.13rem;
                color: #ffffff;
            }
          }
        }
      .footer_c{
        width: 1.28rem;
        height: 0.42rem;
        background-color: #1776af;
        border-radius: 0.06rem 0.06rem 0 0;
        p{
          line-height: 0.42rem;
          text-align: center;
            span:nth-child(1){
              color: #ffffff;
              margin: 0 0.08rem;
              position: relative;
              top: 0.04rem;
            }
            span:nth-child(2){
                font-size: 0.13rem;
                color: #ffffff;
            }
          }
      }
    // }
  }
}
</style>