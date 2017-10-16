<template>
  <header>
    <div class="log"></div>
    <nav>
      <ul>
        <li><a href="#">首页</a></li>
        <li><a href="#">简历</a></li>
        <li class="on"><a href="#">组件</a></li>
        <li><a href="#">模板</a></li>
        <li><a href="#">博客</a></li>
      </ul>
    </nav>
  </header>
</template>

<style lang='scss'>
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  header{
    display: flex; min-height: 80px; background: #fff; margin-bottom: 20px;
    >.log{
      min-width: 20em; padding: 26px 0;
      &:after{
        display: block; content: ""; height: 100%; border-right: 1px solid $borderCor;
      }
    }
    >nav{
      display: flex; justify-content: flex-end; flex: 1;
      >ul{
        display: flex; min-width: 36em;
        >li{
          display: flex; flex-grow: 1; padding: 0 1em;
          a{
             display: flex; width: 100%; height: 100%; align-items: center; justify-content: center; border-bottom: 2px solid transparent;
            &:hover{
              color: $hoverCor; border-bottom-color: $hoverCor;
            }
          }
          &.on{
            a{
              color: $hoverCor; border-bottom-color: $hoverCor;
            }
          }
        }
      }
    }
  }
</style>

<script>

</script>
