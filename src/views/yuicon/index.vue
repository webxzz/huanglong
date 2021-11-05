<template>
  <div class="yuicon">
    <div class="yuicon_conter">
      <div class="yic_img">
        <img src="../../assets/imgs/首页改1_03.gif" alt="" />
      </div>
      <div class="yic_imgone">
        <a-dropdown :trigger="['click']" >
          <a class="ant-dropdown-link" @click="(e) => e.preventDefault()" >
            <svg class="icon" aria-hidden="true">
              <use xlink:href="#icon-list"></use>
            </svg>
          </a>
          <a-menu slot="overlay" class="icon_top"  placement="topRight">
            <a-menu-item key="0">
              <a href="#">煜龙时空</a>
            </a-menu-item>
            <a-menu-item key="1">
              <a href="#">1煜龙时空</a>
            </a-menu-item>
            <a-menu-item key="2">
              <a href="#">2煜龙时空 </a>
            </a-menu-item>
            <a-menu-item key="3">
              <a href="#">3煜龙时空</a>
            </a-menu-item>
            <a-menu-item key="4">
              <a href="#">4煜龙时空</a>
            </a-menu-item>
            <a-menu-item key="5">
              <a href="#">5煜龙时空</a>
            </a-menu-item>
          </a-menu>
        </a-dropdown>
      </div>
    </div>
  </div>
</template>
          

<script>
</script>

<style lang="scss" scoped>
.icon {
  width: 0.3rem;
  height: 0.22rem;
  vertical-align: -0.15em;
  fill: currentColor;
  overflow: hidden;
}
.yuicon {
  width: 3.75rem;
  background: #eaeaea;
  margin: 0 auto;
}
.yuicon_conter {
  display: flex;
  justify-content: space-between;
}
.yic_img {
  width: 1.03rem;
  height: 0.29rem;
  margin: 0.1rem 0 0.095rem 0.1rem;
  img {
    width: 100%;
    height: 100%;
  }
}
.yic_imgone {
  width: 0.3rem;
  height: 0.22rem;
  margin: 0.15rem 0.145rem 0.115rem 0;
}
.icon_top {
    text-align: center;
width: 1.5rem;

position: relative;
top: .07rem;
left: .14rem;
}
</style>>

