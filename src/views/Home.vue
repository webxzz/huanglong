<template>
    <div class="wrap">
          <header class="header">

          </header>
          <main class="main">

          </main>
          <footer class="footer">

          </footer>
    </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
.wrap{
  height: 100%;
  display: flex;
  flex-direction: column;
  .header{
      width: 3.75rem;
      // height: 0.4rem;
      background: red;
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