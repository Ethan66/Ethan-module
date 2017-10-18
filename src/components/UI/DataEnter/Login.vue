<template>
  <form class="e-login">
    <div class="line">
      <label><i class="iconfont icon-user"></i></label>
      <input type="text" placeholder="username" />
    </div>
    <div class="line">
      <label><i class="iconfont icon-mima"></i></label>
      <input type="text" placeholder="password" />
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
    <div class="line">
      <a class="registerBtn" href="">Register now</a>
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
      box-shadow: 0 0 0 2px #fff; text-indent: 26px;
      transition: border-color .6s,box-shadow .3s;
      &:hover{
        border-color: $hoverCor;
      }
      &:focus{
        box-shadow: 0 0 0 2px rgba(16,142,233,.2); border-color: #eee;
      }
    }
    :-moz-placeholder { /* Mozilla Firefox 4 to 18 */
      color: #ccc;
    }

    ::-moz-placeholder { /* Mozilla Firefox 19+ */
      color: #ccc;
    }

    input:-ms-input-placeholder{
      color: #ccc;
    }

    input::-webkit-input-placeholder{
      color: #ccc;
    }
    input[type=submit],.registerBtn{
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
    .registerBtn{
      display: block; line-height: 30px; border: 1px solid $hoverCor; border-radius: 4px; text-align: center;
    }
  }
</style>
