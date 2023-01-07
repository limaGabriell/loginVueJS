<template>
    
</template>

<script>
    export default {
        name: 'FormComponents'
    }
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
    .container {
    width: 100%;
    margin: 0 auto;
}

.container-login { 
    width: 100%;
    min-height: 100vh;

    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;

    background-color: #111;

}

.wrap-login {
    width: 390px;
    background: #333;
    border-radius: 20px;

    overflow: hidden;
    padding: 77px 55px 33px 55px;

    box-shadow: 0px 5px 10px 0px rgba(0, 255, 34, 0.514);
}

.login-form{
    width: 100%;
}

.login-form-title{
    display: block;
    font-size: 30px;
    color: azure;

    line-height: 1.2;
    text-align: center;
}

.login-form-title img {
    width: 90px;
}

.wrap-input {
    width: 100%;
    position: relative;
    border-bottom: 2px solid #adadad;
    margin-bottom: 37px;
}

.wrap-input input {
    font-size: 15px;
    color: #fff;
    line-height: 1.2;
    border: none;
    display: block;

    width: 100%;
    height: 45px;

    background-color: transparent;
    padding: 0 5px;
}

.focus-input {
    position: absolute;
    display: block;
    width: 100%;
    height: 100%;

    top: 0;
    left: 0;

    pointer-events: none;
    color: #adadad;
}

.focus-input::before {
    content: "";
    display: block;
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;

    -webkit-transition: all 0.4s;
    -o-transition: all 0.4s;
    -moz-transition: all 0.4s;

    background: -webkit-linear-gradient(to left, #01ff01, #048804);
    background: -o-linear-gradient(to left, #01ff01, #048804);
    background: -moz-linear-gradient(to left, #01ff01, #048804);
    background: linear-gradient(to left, #01ff01, #048804);
}
.focus-input::after {
    font-size: 15px;
    color: #999999;
    line-height: 1.2;
    
    content: attr(data-placeholder);
    
    display: block;
    width: 100%;
    position: absolute;
    top: 16px;
    left: 0px;
    padding-left: 5px;

    -webkit-transition: all 0.4s;
    -o-transition: all 0.4s;
    -moz-transition: all 0.4s;
  }

  input:focus {
    outline: 0;
  }
  
  input:focus + .focus-input::after {
    top: -15px;
  }

  input:focus + .focus-input::before {
    width: 100%;
  }

  .has-val + .focus-input::after {
    top: -15px;
  }

  .has-val + .focus-input::before {
    width: 100%;
  }

  .container-login-form-btn {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding-bottom: 13px; 
  }

  .login-form-btn {
    font-size: 15px;
    border: none;
    border-radius: 10px;
    color: #fff;
    
    line-height: 1.2;

    text-transform: uppercase;
    font-weight: bold;

    display: flex;
    justify-content: center;
    align-items: center;

    width: 100%;
    height: 50px;

    background: -webkit-linear-gradient(to left, #01ff01, #048804);
    background: -o-linear-gradient(to left, #01ff01, #048804);
    background: -moz-linear-gradient(to left, #01ff01, #048804);
    background: linear-gradient(to left, #01ff01, #048804);
  }

.login-form-btn:hover {
    cursor: pointer;
}

.text-account {
    display: flex;
    justify-content: center;
    padding-top: 10px;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 17px;
}

.txt1 {
    color: #fff;
    padding-right: 10px;
}

.txt2 {
    color: #01ff01;
    text-decoration: none;
}
</style>