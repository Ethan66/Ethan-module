<template>
  <div class="e-dropdown2">
    <a href="javascript:void(0)">Click me</a>
    <ul>
      <li><a href="">Click me1</a></li>
      <li><a href="">Click me2</a></li>
      <li><a href="">Click me3</a></li>

    </ul>
  </div>
</template>

<script>
  var show=function(){
    alert(1);
  }
</script>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .e-dropdown2{
    display: inline-block; padding-right: 20px; position: relative;
    >a{
      color: $hoverCor; position: relative;
      &::after{
        display: block; content: ""; width: 6px; height: 6px; border: 1px solid {left:0;bottom:0;}; color: inherit;
        position: absolute; right: -15px; top: 4px; transform: rotate(135deg);
      }
    }
    >ul{
      height:0; opacity: 0; overflow: hidden; border-radius: 3px; color: #666; line-height: 26px; text-align: center;
      background: #fff; white-space: nowrap;
      position: absolute; left: -2px; z-index: 1000; transition: 0.3s all;
      >li{
        padding: 4px 8px;
      }
      a:hover{
        color: $hoverCor;
      }
    }
    &:hover>ul{
       height: 102px; box-shadow: 0 1px 3px rgba(0,0,0,.1); border: 1px solid $borderCor; opacity:1;
    }
  }
</style>



