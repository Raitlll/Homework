<template>
  <div id="nav">
    <div>
      <img id="logo" src="src/assets/sticky-notes.png">
    </div>
    <div>
      <router-link to="/main">Home</router-link> |
      <router-link to="/about">Contact Us</router-link> |
      <router-link to="/login">Login</router-link>
    </div>
  <!-- <div class="Search">
      <form>
        <input type="text" id="searchbar">
        <input type="submit" id="submit" value="Search">
      </form>
    </div> -->

  </div>
  <router-view />
  <div id="footer">
    <router-link to="/about">Contact Us</router-link>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 20px;

  a {
    font-weight: bold;
    color: whitesmoke;

    &.router-link-exact-active {
      color: #f49f1c;
    }
  }
  border-bottom: solid whitesmoke;
}

#footer {
  position: relative;
  bottom: 0;
  width: 100%;
  margin-top: 20px;
  margin-bottom: 20px;
  a{
    font-weight: bold;
    color: whitesmoke;
    &.router-link-exact-active {
      color: #f49f1c;
    }
  }
}

#logo{
  float: left;
  height: 40px;
}
#userpic{
  height: 40px;
  float: right;
}
.Search{
  float: right;
  margin: auto;
  align-self: center;
  text-align: center;
}
body{
  background-color: #00172D;
}
</style>
