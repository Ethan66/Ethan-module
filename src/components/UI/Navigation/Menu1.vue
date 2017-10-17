<template>
  <header class="e-header">
    <div class="log">LOGO</div>
    <nav>
      <ul>
        <li><a href="">Index Page</a></li>
        <li><a href="">Page Tow</a></li>
        <li class="on"><a href="">Page three</a></li>
        <li>
          <a href="javascript:void(0)">Page four</a>
          <ul class="list">
            <li><a href="#">List One</a></li>
            <li><a href="#">List Two</a></li>
            <li><a href="#">List Three</a></li>
          </ul>
        </li>
        <li><a href="">Page five</a></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .e-header{
    display: flex; min-height: 34px; background: #fff; margin-bottom: 0;
    >.log{
      min-width: 20%; padding: 8px 0;
      &:after{
        display: inline-block; content: ""; height: 100%; border-right: 1px solid $borderCor; float: right;
      }
    }
    >nav{
      display: flex; justify-content: flex-end; flex: 1;
      >ul{
        display: flex; min-width: auto;
        >li{
          display: flex; flex-grow: 1; padding: 0 1em; position: relative;
          >a{
            display: flex; width: 100%; height: 100%; align-items: center; justify-content: center; border-bottom: 2px solid transparent;
          }
          &:hover{
            color: $hoverCor; border-bottom-color: $hoverCor;
          }
          &.on{
            a{
              color: $hoverCor; border-bottom-color: $hoverCor;
            }
          }
          .list{
            height: 0; opacity: 0; overflow: hidden; border-radius: 3px; color: #666; line-height: 26px;
            text-align: center; background: #fff; white-space: nowrap;
            position: absolute; left: 8px; top: 36px; z-index: 1000; transition: 0.3s all;
            >li{
              padding: 4px 8px;
              & a:hover{
                border-bottom-color: #fff;
              }
            }
          }
          &:hover .list{
            height: 108px; box-shadow: 0 1px 3px rgba(0,0,0,.1); border: 1px solid $borderCor; opacity:1;
          }
        }
      }
    }
  }
</style>
