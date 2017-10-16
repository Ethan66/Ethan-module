<template>
  <nav class="nav">
    <ul>
      <li>
        <a class="title subUl" href="#">Navigation</a>
        <ul class="list">
          <li class="on"><a href="#">Breadcrumb<span>面包屑</span></a></li>
          <li><a href="#">Dropdown<span>下拉菜单</span></a></li>
          <li><a href="#">Menu<span>导航</span></a></li>
          <li><a href="#">Steps<span>步骤条</span></a></li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<style lang='scss'>
  $borderCor:#e9e9e9; $hoverCor:#108ee9; $opacityCor: rgba(16,142,233,.1);
  @mixin after{
    display: block; content:'';
  }
  .nav{
    min-width: 22em; background: #fff;
    .title{
      display: block; width: 100%; height: 46px; line-height: 46px; padding-left: 24px; font-size: 16px; position: relative;
      &:hover{
        color: $hoverCor;
      }
    }
    .subUl::after{
      display: block; content:""; width: 8px; height: 8px; border: 1px solid #999{top:0;right: 0;}
      position: absolute; top: 0; right: 0; transform: rotate(135deg); top: 20px; right: 20px;
    }
    .list{
      >li{
        height: 36px; line-height: 36px; color: #666; border-right: 3px solid transparent;
        a{
          display: block; width: 100%; padding-left: 2.6em;
          span{
            color: #999; padding-left: 1em;
          }
        }
        &.on{
          background:$opacityCor; border-right-color: $hoverCor;
        }
      }
    }
  }
</style>
