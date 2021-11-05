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

          </main>
          <footer class="footer">

          </footer>
    </div>
</template>

<script>
import Yuicon from '@/views/yuicon'
import Lunbo from '@/views/lunbo/lunbo.vue'
  export default {
    components: {
        Yuicon,
        Lunbo
     },
      data(){
        return{
          inp:''
        }
      }
  }
</script>

<style lang="scss" scoped>
input{
  background:none;  
	outline:none;  
	border:none;
}
.wrap{
  height: 100%;
  display: flex;
  flex-direction: column;
  .header{
      width: 3.75rem;
      // height: 0.4rem;
      background: red;
      margin: 0 auto;
      .header_top{
        width: 3.75rem;
        height: 0.3rem;
        background: #fff;
        // display: flex;
        // align-items: center;
        p{
          width: 2.80rem;
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
    //  overflow-y: scroll;
  }
  .footer{
    width: 3.75rem;
    height: 0.4rem;
    background: red;
    margin: 0 auto;
  }
}
</style>