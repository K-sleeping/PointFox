<template>
  <div id="registerWrapper">
      <!-- crtl + F    可以全文找词替换 -->
    <div id="registerContent">
      <el-card class="box-card">
        <div slot="header" class="clearfix">
          <span>用户注册</span>
          <!-- <el-button style="float: right; padding: 3px 0" type="text"
            >忘记密码</el-button
          > -->
        </div>
        <div id="loginContent">
          <el-input id="username" v-model="newuser.username" clearable></el-input>
          <el-input id="password" v-model="newuser.password" clearable show-password></el-input>
        </div>
        <div id="submitContent">
          <el-button id="systemSubmit">注册</el-button>
        </div>

      </el-card>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      newuser:{
        username:"",
        password:""
      }
    }
  }
};
</script>

<style>
#registerWrapper {
  /* background-color: pink; */
  padding-top:100px;
}
#registerContent{
  width:400px;
  margin: 0 auto;
}
#password{
  margin: 5px 0;
}
#systemSubmit{
    display: block;
    background-color: #0a9588  !important;
    border-color:#0a9588  !important;
    color:white  !important;
    margin:0 auto;
}
</style>