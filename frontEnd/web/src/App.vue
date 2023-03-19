<template>
  <div>
    <h1 class="title">GestureGraphix</h1>
    <div class="contents">
      <form>
        <label for="id">ID</label>
        <input type="text" name="id" id="id" required="required">
      </form>
      <form>
        <label for="pw">PW</label>
        <input type="password" name="pw" id="pw" required="required">
      </form>
      <button>LOG IN</button>
      <div class="options">
        <p>아직 회원이 아니신가요? <a href="#">회원가입하기</a></p>
        <p><a href="#">ID & PW 찾기</a></p>
      </div>
    </div>
    <p class="copy">ⓒ 2023. JunBeul. All rights reserved.</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {

  }
}
</script>

<style>
@import 'https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css';
@import url(https://cdn.jsdelivr.net/gh/moonspam/NanumSquare@2.0/nanumsquare.css);
#app {
  width: 100vw;
  height: 100vh;
  background-image: url(./assets/bg.png);
  background-size: 100%;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'NanumSquare', sans-serif;
}
h1.title{
  text-align: center;
  font-size: 64px;
  font-weight: 800;
  letter-spacing: 8px;
  margin-right: -8px;
  margin-bottom: 25px;
  color: #6FAAE7;
}
.contents{
  width: 600px;
  height: 400px;
  margin-bottom: 25px;
  
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  background: rgba( 255, 255, 255, 0.25 );
  box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
  backdrop-filter: blur( 4px );
  -webkit-backdrop-filter: blur( 4px );
  border-radius: 18px;
  border: 1px solid rgba( 255, 255, 255, 0.18 );
}
form{
  width: 490px;
  height: 40px;
  margin-bottom: 25px;
}
label{
  display: inline-block;
  margin: 0;
  padding: 0;
  width: 40px;
  height: 40px;
  text-align: center;
  font-size: 16px;
}
input{
  width: 450px;
  height: 40px;
  margin: 0;
  padding: 11px 20px;
  box-sizing: border-box;
  border-radius: 20px;
  border: solid 2px #fff;
  background-color: #fff;
  font-size: 16px;
}
input:focus {
  outline: none;
  background-color: #fff0;
}
input:valid,
input:focus {
  background-color: #fff0;
}
button{
  width: 140px;
  height: 60px;
  margin-bottom: 25px;
  border: none;
  border-radius: 18px;
  background: linear-gradient( 45deg, #6FAAE7, #FBC0FF );
  color: #fff;
  font-size: 16px;
  font-weight: 800;
  font-family: 'NanumSquare', sans-serif;
  cursor: pointer;
}
.options{
  text-align: center;
}
.options > p:first-child{
  margin-bottom: 10px;
}
.options > p > a{
  color: #6FAAE7;
}
.copy{
  width: 600px;
  text-align: center;
  font-size: 12px;
}
</style>
