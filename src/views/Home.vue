<template>
    <div class="wrap">
          <header class="header">
              <div class="header_top">
                <input type="text" v-model="inp" placeholder="欢迎来到紧缺应用技术技能型人才职业教育报考平台">
              </div>
          </header>
          <main class="main">

          </main>
          <footer class="footer">

          </footer>
    </div>
</template>

<script>
  export default {
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
      .header_top{
        width: 3.75rem;
        height: 0.3rem;
        background: paleturquoise;
        display: flex;
        input{
          width: 275px;
          height: 0.3rem;
          font-family: PingFang-SC-Medium;
          font-size: 12px;
          font-weight: normal;
          font-stretch: normal;
          letter-spacing: 0px;
          color: #777777;
          margin: 0 0 0 0.13rem;

        }
      }
  }
  .main{
     flex: 1;
     overflow-y: scroll;
  }
  .footer{
    width: 3.75rem;
    height: 0.4rem;
    background: red;
  }
}
</style>