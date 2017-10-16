<template>
  <nav class="nav">
    <ul>
      <li>
        <a class="title subUl" href="#">Navigation</a>
        <ul class="list">
          <li><a href="#">Breadcrumb</a><span>面包屑</span></li>
          <li><a href="#">Dropdown</a><span>下拉菜单</span></li>
          <li><a href="#">Menu</a><span>导航</span></li>
          <li><a href="#">Steps</a><span>步骤条</span></li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<style lang='scss'>
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  @mixin after{
    display: block; content:'';
  }
  .nav{
    max-width: 16em; background: #fff;
    .title{
      display: block; width: 100%; height: 50px; line-height: 50px; padding-left: 20px; font-size: 16px; position: relative;
      &:hover{
        color: $hoverCor;
      }
    }
    .subUl::after{
      display: block; content:""; width: 8px; height: 8px; border: 1px solid #999{top:0;right: 0;}
      position: absolute; top: 0; right: 0; transform: rotate(135deg); top: 18px; right: 12px;
    }
    .list{
      >li{
        padding-left: 2.4em; height: 34px; line-height: 30px; color: #666;
        span{
          color: #999; padding-left: 1em;
        }
      }
    }
  }
</style>
