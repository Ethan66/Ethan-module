<template>
  <form class="e-login">
    <div class="line">
      <label><i class="iconfont icon-user"></i></label>
      <input type="text"  />
    </div>
    <div class="line">
      <label><i class="iconfont icon-mima"></i></label>
      <input type="text"  />
    </div>
    <div class="line text">
      <p>
        <label>
          <input type="checkbox" />Remember me
        </label>
        <a href="">Forgot password</a>
      </p>
    </div>
    <div class="line">
      <input type="submit" value="Login" />
    </div>
  </form>
</template>

<style lang='scss'>
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .e-login{
    display: inline-block;
    .line{
      margin-bottom: 20px; position: relative;
    }
    label{
      position: absolute; top: 6px; left: 6px; color: #999;
    }
    input{
      border: 1px solid #ddd; border-radius: 4px; line-height: 30px; width: 20em; text-indent: 10px;
      box-shadow: 0 0 0 2px #fff;
      transition: border-color .6s,box-shadow .6s;
      &:hover{
        border-color: $hoverCor;
      }
      &:focus{
        box-shadow: 0 0 0 2px rgba(16,142,233,.2);
      }
    }
    input[type=submit]{
      padding: 0 12px; text-indent: 0; background: $hoverCor; color: #fff;
      outline: 0; border-color: $hoverCor; cursor: pointer; transition: all .3s;
      &:hover{
        background: #49a9ee; border-color: #49a9ee;
      }
    }
    .text{
      margin-bottom: 5px;
      label{
        position: static;
      }
      input[type=checkbox]{
        width: auto; margin-right: 3px; vertical-align: -1px;
        &:focus{
          box-shadow: none;
        }
      }
      a{
        float: right; color: $hoverCor;
      }
    }
  }
</style>
