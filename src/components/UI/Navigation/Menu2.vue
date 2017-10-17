<template>
  <nav class="e-nav2">
    <ul class="clearfix">
      <li><a href="">Index Page</a></li>
      <li><a href="">Page Tow</a></li>
      <li class="on"><a href="">Page three</a></li>
      <li>
        <a href="javascript:void(0)">Page four <span></span><i></i></a>
        <div class="bgwhite">
          <ul class="list">
            <li><a href="#">List One</a></li>
            <li><a href="#">List Two</a></li>
            <li><a href="#">List Three</a></li>
          </ul>
        </div>
      </li>
      <li><a href="">Page five</a></li>
    </ul>
  </nav>
</template>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .clearfix:after{
    display: block; content:""; clear: both;
  }
  .e-nav2{
    height: 36px; line-height: 36px; background: $hoverCor; color: #fff; position: relative;
    >ul{
      width: 80%; height: 100%; margin: 0 auto;
    }
    >ul>li{
      padding: 0 20px; height: 100%; float: left; background: transparent;
      transition: all 0.4s;
      >a{
        display: block; width: 100%; height: 100%; position: relative;
        span{
          display: block; width: 6px; height: 6px; border: 2px solid #fff{left: 0; bottom: 0;};
          position: absolute; right: -12px; top: 14px;
          transform: rotate(135deg); transition: all 0.2s;
        }
        i{
          display: block; width:0; height: 0; border: 5px solid transparent; opacity: 0;
          border-bottom-color: #fff; box-sizing: content-box;
          position: absolute; bottom: 0; left: 50%; transition: all 0.1s;
        }
      }
      &:hover{
        background: #0d76c1;
        .bgwhite{
          opacity: 1;
        }
        span{
          transform: rotate(-405deg); top: 16px;
        }
        i{
          opacity: 1;
        }
      }
    }
    .bgwhite{
      width: 100%; height: 34px; line-height: 34px; background: #fff; opacity: 0;
      position: absolute; bottom: -34px; left: 0; z-index: 1000;
      box-shadow: 0 3px 3px rgba(0,0,0,.1);
      .list{
        width: 80%; margin: 0 auto;
        li{
          padding: 0 20px; color: #666; float: left;
          &:hover{
            color: $hoverCor;
          }
        }
      }
    }
  }
</style>
