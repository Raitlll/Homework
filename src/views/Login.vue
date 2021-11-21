<template>
  <div>
    <h1>Log in here</h1>
  </div>
  <div class="login">
    <div class="loginBox">
      <form id="login">
        <p>Username:</p>
        <input type="text" id="email" value="" />
        <br />
        <p>Password:</p>
        <input type="text" id="password" value="" />
        <br />
        <br />
        <input type="submit" value="Submit" />
        <br />
        <br />
        <a href="">Forgot password?</a>
      </form>
    </div>
  </div>
</template>

<script>
//import LoginPage from "@/components/LoginPage";
export default {
  name: "Login",
};
</script>

<style scoped>
.loginBox {
  border-style: solid;
  border-color: whitesmoke;
  margin: 10px;
}
form p {
  font-weight: bold;
}
input[type="submit"],
input[type="text"] {
  border-radius: 5px;
  font-size: 18px;
}
input[type="submit"] {
  background-color: #2c3e50;
  color: #f49f1c;
  border: none;
  cursor: pointer;
}
.loginBox {
  background-color: #f49f1c;
}
h1 {
  color: #f49f1c;
}
</style>
