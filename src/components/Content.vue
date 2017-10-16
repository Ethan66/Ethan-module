<template>
  <div class="content">
    <div class="headline">
      <h2 class="tit">Breadcrumb面包屑<i class="iconfont icon-timu"></i></h2>
      <p>显示当前页面在系统层级结构中的位置，并能向上返回。</p>
    </div>
    <div class="code">
      <h2 class="tit">代码演示<i class="iconfont icon-gongneng"></i></h2>
      <div class="col-6 border">
        <Nav />
      </div>
      <div class="col-6 border"></div>
    </div>
  </div>
</template>

<script>
  import Nav from './UI/Navigation.vue'
  export default {
    name:"Content",
    components:{
      Nav
    }
  }
</script>


<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  h2.tit{
    font-weight: normal; font-size: 24px; margin: 20px 0 16px;
    .iconfont{
      color: #999; font-size: 14px; margin-left: 10px;
    }
  }
  .code .tit .iconfont{
    vertical-align: 3px;
  }
  .headline{
    margin-bottom: 50px;
    p{
      color: #666;
    }
  }
  .col-6{
    width: 48%;
  }
  .border{
    border: 1px solid $borderCor; border-radius: 5px;
  }
</style>

