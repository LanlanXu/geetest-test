<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="scss">
html,
body {
  padding: 0;
  margin: 0;
  background: #ff5b62;
}

.msg {
  background: #000;
  color: #fff;
  text-align: center;
  line-height: 1.6rem;
  padding: 0.4rem 0;
  position: fixed;
  width: 70%;
  top: 45%;
  left: 15%;
  border-radius: 0.5rem;
  box-shadow: 0 0 0.3rem #d8d6d4;
  z-index: 99999;
}

.fade-enter-active {
  transition: all .2s ease;
}

.fade-leave-active {
  transition: all .1s;
}

.fade-enter,
.fade-leave-to {
  transform: translateY(-10px);
  opacity: 0;
}

input {
  outline: none;
}

@media screen and (max-width:720px) {
  html {
    font-size: 12px !important;
  }
}

@media screen and (min-width:720px) {
  html {
    font-size: 12px !important;
  }
  .landing,
  .links {
    max-width: 400px;
  }
  .landing {
    padding: 0 0 2rem!important;
  }
  .msg {
    max-width: 200px;
    left: calc(50% - 100px);
  }
}

.landing {
  background: #fff;
  border-radius: 5px;
  width: 90%;
  margin: calc(40vh - 7rem) auto 0;
  padding-bottom: 1.4rem;

  .title {
    font-size: 1.2rem;
    font-weight: bold;
    text-align: center;
    color: #ff5a60;
    background: #fdfbfb;
    line-height: 3.2rem;
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
  }
  .login {
    padding: 0 1rem;

    .item {
      line-height: 3.2rem;
      padding: 0.6rem 0 0 0.7rem;
      font-size: 0;
      border-bottom: 1px solid #ddd;

      .imgCode {
        width: 6.8rem;
        height: 2.4rem;
        vertical-align: middle;
        margin-right: 0;
      }

      label {
        font-size: 1.1rem;
        color: #666;
        height: 2.4rem;
        line-height: 2.4rem;
        vertical-align: middle;
        display: inline-block;
        width: 24%;
      }

      input {
        border: none;
        font-size: 1.1rem; // vertical-align: middle;
        height: 2.4rem;
        line-height: 2.4rem;
        width: calc(100% - 1.2rem);
        vertical-align: middle;
      }

      .close {
        width: 1.2rem;
        height: 1.2rem;
        vertical-align: middle;
      }
    }
  }

  .main-btn {
    line-height: 2.8rem;
    text-align: center;
    background: #ff5a60;
    color: #fff;
    border-radius: 0.2rem;
    font-size: 1.1rem;
    display: block;
    width: 90%;
    margin: 1.4rem auto 0;
  }
}

.links {
  width: 90%;
  margin: 0 auto;
  text-align: right;
  line-height: 3.2rem;
  a {
    padding: 0 1rem;
    color: #fff;
    text-decoration: none;
  }
}

.default-input {
  display: inline-block;
  width: 76%;
}
</style>
