<template>
  <div class="content">
    <div id="crumb">
      <div class="headline">
        <h2 class="tit">Breadcrumb面包屑<i class="iconfont icon-timu"></i></h2>
        <p>显示当前页面在系统层级结构中的位置，并能向上返回。</p>
      </div>
      <div class="code">
        <h2 class="tit">功能演示<i class="iconfont icon-gongneng"></i></h2>
        <div class="col-6 border">
          <div class="show">
            <Breadcrumb />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用after伪元素添加></p>
          </div>
        </div>
        <div class="col-6 border">
          <div class="show">
            <Breadcrumb2 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用after伪元素添加/</p>
          </div>
        </div>
      </div>
    </div>
    <div id="dropdown">
      <div class="headline">
        <h2 class="tit">Dropdown下拉菜单<i class="iconfont icon-timu"></i></h2>
        <p>向下弹出的列表。</p>
      </div>
      <div class="code">
        <h2 class="tit">功能演示<i class="iconfont icon-gongneng"></i></h2>
        <div class="col-6 border">
          <div class="show">
            <Dropdown1 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>css3过渡，需要设置ul高度</p>
          </div>
        </div>
        <div class="col-6 border">
          <div class="show">
            <Dropdown2 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>css3过渡，需要设置ul高度</p>
          </div>
        </div>
      </div>
    </div>
    <div id="menu">
      <div class="headline">
        <h2 class="tit">Menu导航菜单<i class="iconfont icon-timu"></i></h2>
        <p>为页面和功能提供导航的菜单列表。</p>
      </div>
      <div class="code">
        <h2 class="tit">功能演示<i class="iconfont icon-gongneng"></i></h2>
        <div class="col-12 border">
          <div class="show">
            <Menu1 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>flex布局，适合企业官网，左右宽度自定义</p>
          </div>
        </div>
        <div class="col-12 border">
          <div class="show">
            <Menu2 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用float布局</p>
          </div>
        </div>
      </div>
    </div>
    <div id="steps">
      <div class="headline">
        <h2 class="tit">Steps步骤条<i class="iconfont icon-timu"></i></h2>
        <p>引导用户按照流程完成任务的导航条。</p>
      </div>
      <div class="code">
        <h2 class="tit">功能演示<i class="iconfont icon-gongneng"></i></h2>
        <div class="col-12 border">
          <div class="show">
            <Step1 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用flex布局</p>
          </div>
        </div>
        <div class="col-12 border">
          <div class="show">
            <Step2 />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用float布局</p>
          </div>
        </div>
      </div>
    </div>
    <div id="register">
      <div class="headline">
        <h2 class="tit">表单域<i class="iconfont icon-timu"></i></h2>
        <p>用户注册和登录页面</p>
      </div>
      <div class="code">
        <h2 class="tit">功能演示<i class="iconfont icon-gongneng"></i></h2>
        <div class="col-12 border">
          <div class="show">
            <Register />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用float布局</p>
          </div>
        </div>
        <div class="col-12 border">
          <div class="show">
            <Login />
          </div>
          <div class="notice">
            <h4>备注<i class="iconfont icon-z-pencil"></i></h4>
            <p>使用float布局</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Breadcrumb from './UI/Navigation/Breadcrumb'
  import Breadcrumb2 from './UI/Navigation/Breadcrumb2'
  import Dropdown1 from './UI/Navigation/Dropdown1'
  import Dropdown2 from './UI/Navigation/Dropdown2'
  import Menu1 from './UI/Navigation/Menu1'
  import Menu2 from './UI/Navigation/Menu2'
  import Step1 from './UI/Navigation/Step1'
  import Step2 from './UI/Navigation/Step2'
  import Register from './UI/DataEnter/Register'
  import Login from './UI/DataEnter/Login'
  export default {
    name:"Content",
    components:{
      Breadcrumb,Breadcrumb2,Dropdown1,Dropdown2,Menu1,Menu2,Step1,Step2,
      Register,Login
    }
  }
</script>


<style lang="scss">
  $borderCor:#e9e9e9; $hoverCor:#108ee9;
  .content>div{
    border-top: 1px solid transparent;
  }
  h2.tit{
     width: 100%; font-weight: normal; font-size: 24px; margin: 20px 0 16px;
    .iconfont{
      color: #aaa; font-size: 14px; margin-left: 10px;
    }
  }
  .code .tit .iconfont{
    vertical-align: 3px;
  }
  .headline{
    margin-bottom: 35px;
    p{
      color: #666;
    }
  }
  .col-12{
    width: 100%;
  }
  .col-6{
    width: 48%;
  }
  .icon-z-pencil{
    font-size: 14px; margin-left: 6px;
  }
  .border{
    border: 1px solid $borderCor; border-radius: 5px; margin-bottom: 20px;
  }
  .code{
    display: flex; flex-wrap: wrap; justify-content: space-between; margin-bottom: 45px;
    .show{
      padding: 40px 20px;
    }
    .notice{
      padding: 20px; border-top: 1px solid $borderCor; color: #888; position: relative;
      h4{
        display: inline-block; font-size: 14px; font-weight: normal; background: #fff; padding: 0 8px;
        position: absolute; left: 14px; top: -9px;
      }
    }
  }
</style>

