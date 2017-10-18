<template>
  <form class="e-register">
    <div class="line">
      <label>
        <span class="tit">Username</span>
        <input type="text" />
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Name</span>
        <input type="text" />
        <i class="e-notice">填写真实姓名</i>
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Phone Number</span>
        <input type="text" />
        <i class="e-notice">填写常用手机号</i>
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Captcha</span>
        <input type="text" class="width50" />
        <button>Get Captcha</button>
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Email</span>
        <input type="text" />
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Password</span>
        <input type="password" />
        <i class="e-notice">长度8-16位，须包含数字、英文字母</i>
      </label>
    </div>
    <div class="line">
      <label>
        <span class="tit">Confirm Password</span>
        <input type="password" />
      </label>
    </div>
    <div class="line marginL">
      <p class="min-text">
        <label>
          <input type="checkbox" />I have read the <a href="">agreement</a>
        </label>
      </p>
      <input type="submit" value="Register" />
    </div>
  </form>
</template>

<style lang='scss'>
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .e-register{
    .width50{
      width: 180px;
    }
    .e-notice{
      font-style: normal; color: #999; margin-left: 10px;
    }
    .line{
      margin-bottom: 15px;
    }
    .tit{
      display: block; float: left; width: 10em; text-align: right; padding-right: 16px; line-height: 30px;
      color: #666;
      &::before{
        display: inline; content: "*"; color: red; margin-right: 3px;
      }
    }
    input{
      border: 1px solid #ddd; border-radius: 4px; line-height: 30px; width: 20em; text-indent: 10px;
      box-shadow: 0 0 0 2px transparent;
      transition: border-color .6s,box-shadow .3s;
      &:hover{
        border-color: $hoverCor;
      }
      &:focus{
        box-shadow: 0 0 0 2px rgba(16,142,233,.2); border-color: #eee;
      }
    }
    button{
      border: 1px solid #ddd; background: #fff; border-radius: 4px; padding: 7px 6px; color: #666;
      transition: all .3s;
      &:hover{
        color: $hoverCor; border-color: $hoverCor; cursor: pointer;
      }
    }
    input[type=submit]{
      width: auto; padding: 0 12px; text-indent: 0; background: $hoverCor; color: #fff;
      outline: 0; border-color: $hoverCor; cursor: pointer;
    }
    input[type=checkbox]{
      width: auto; margin-right: 10px; vertical-align: -1px;
      &:focus{
        box-shadow: none;
      }
    }
  .marginL{
    margin-left: 10em;
  }
    .min-text {
      margin-bottom: 10px; color: #666;
      label {
        width: auto;
      }
      a{
        color: $hoverCor;
      }
    }
  }
</style>
