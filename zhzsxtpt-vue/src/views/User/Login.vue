<template>
  <div
    class="loginPage"
    :style="{
      backgroundImage: 'url(' + require('@/assets/images/loginbg.png') + ')'
    }"
  >
    <div
      class="logo"
      :style="{
        backgroundImage: 'url(' + require('@/assets/images/logo.png') + ')'
      }"
    ></div>
    <div class="title">
      <h1>指挥值守系统平台</h1>
      <h5>Command and duty system platform</h5>
    </div>
    <div class="loginBlock">
      <div class="login_input login_username"><input type="text" /></div>
      <div class="login_input login_password"><input type="password" /></div>
      <div class="row">
        <div class="col_12">
          <i class="checkBox icon-checkbox-unchecked"> 记住密码</i>
        </div>
        <div class="col_12 tar"><a-button type="primary">登 录</a-button></div>
      </div>
    </div>
    <div class="copyright">
      <div>Copyright © 2020-2022 辽宁省司法厅</div>
      <div>Powered By 方正国际软件有限公司 v1.0</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style>
.loginPage {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 10000;
  background-size: cover;
  background-color: #29f;
}
.loginPage > div {
  position: absolute;
  right: 0;
  left: 0;
  margin: 0 auto;
}
.loginPage .logo {
  background-position: center;
  background-repeat: no-repeat;
  background-size: auto 100%;
  height: 35%;
  top: 10%;
}
.loginPage .title {
  top: 45%;
  text-align: center;
}
.loginPage .title h1 {
  font-size: 2.4rem;
  line-height: 1;
  color: #fff;
  text-shadow: rgba(0, 0, 0, 0.6) 0 0.2rem 0.2rem;
  font-weight: normal;
  margin-bottom: 0.5rem;
}
.loginPage .title h5 {
  font-size: 0.6rem;
  line-height: 1;
  color: #fff;
  text-shadow: rgba(0, 0, 0, 0.6) 0 0.2rem 0.2rem;
  font-weight: normal;
  text-transform: uppercase;
  letter-spacing: 0.3em;
}
.loginPage .loginBlock {
  width: 22rem;
  height: 12rem;
  top: 55%;
  background-color: #fff;
  border-radius: 0.3rem;
  box-shadow: rgba(0, 0, 0, 0.6) 0 0.2rem 0.2rem;
  box-sizing: border-box;
  padding: 2rem 1.5rem;
}
.loginPage .loginBlock .login_input {
  position: relative;
  border: #ccc solid 1px;
  background-color: #f8f8f8;
  border-radius: 0.2rem;
  padding: 0.1rem 0.1rem 0.1rem 2rem;
  margin-bottom: 1.2rem;
}
.loginPage .loginBlock .login_input input {
  border: none;
  background: none;
  width: 100%;
  padding: 0;
}
.loginPage .loginBlock .login_input::before {
  position: absolute;
  font-family: "iconfounts" !important;
  top: 0;
  bottom: 0;
  left: 0.5rem;
  color: #999;
  height: 1rem;
  font-size: 1rem;
  margin: auto 0;
}
.loginPage .loginBlock .login_username::before {
  content: "\e935";
}
.loginPage .loginBlock .login_password::before {
  content: "\e97d";
}
.loginPage .loginBlock .row div {
  line-height: 1.4rem;
}
.loginPage .loginBlock .row div i {
  color: #bbb;
  font-size: 0.6rem;
}
.loginPage .copyright {
  bottom: 10%;
  text-align: center;
}
.loginPage .copyright div {
  color: #fff;
  font-size: 0.6rem;
}
</style>
