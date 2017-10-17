<template>
  <div class="e-step2">
    <ul class="clearfix">
      <li class="finish clearfix">
        <p class="circle">
          <i>1</i>
        </p>
        <div class="text">
          <h4>Finish</h4>
          <p>This is a description</p>
        </div>
      </li>
      <li class="doing clearfix">
        <p class="circle">
          <i>2</i>
        </p>
        <div class="text">
          <h4>Doing</h4>
          <p>This is a description</p>
        </div>
      </li>
      <li class="waiting clearfix">
        <p class="circle">
          <i>1</i>
        </p>
        <div class="text">
          <h4>Waiting</h4>
          <p>This is a description</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .clearfix::after{
    display: block; content: ""; clear: both;
  }
  .e-step2{
    i{
      font-style: normal;
    }
    >ul{
      >li{
        float: left; width: 38%; margin-right: 10px; position: relative;
        &::after{
          display: block; content: ""; width: 100%; border-top: 1px solid;
          position: absolute; top: 50%; z-index: 1;
        }
        &:last-child{
          width: auto;
        }
      }
    }
    .finish{
      .circle{
        border-color: $hoverCor; color: $hoverCor;
      }
      &::after{
        border-top-color: $hoverCor;
      }
    }
    .doing {
      .circle {
        background: $hoverCor; color: #fff; border-color: $hoverCor;
      }
      &::after {
        border-top-color: #ccc;
      }
    }
    .circle{
      float: left; width: 2.2em; height: 2.2em; border: 1px solid #999; border-radius: 50%; line-height: 2.2em; text-align: center;
      background: #fff; position: relative; z-index: 3;
    }
    .text{
      float: left; padding: 0 10px; background: #fff; position: relative; z-index: 3;
      h4{
        font-size: 16px;
      }
    }
  }
</style>
