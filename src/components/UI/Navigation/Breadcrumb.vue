<template>
  <div class="e-crumb">
    <a href="/">首页</a>
    <a href="">酒店</a>
    <a href="">杭州</a>
    绿藤假日酒店
  </div>
</template>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .e-crumb{
    width: 100%;
    a{
      color: #666;
      &::after{
        display: inline; content: ">"; padding: 0 6px; color: #333;
      }
      &:hover{
        color: $hoverCor;
      }
    }
  }
</style>

