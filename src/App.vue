<template>
  <div id="app">
    <nav class="main-nav">
      <Burger></Burger>
      <button class="button">
        <img src="messaging.jpg">
      </button>
      <button class="button">
        <img src="videocall.jpg">
      </button>
      <button class="button">
        <img src="headphones.jpg">
      </button>
    </nav>

    <Sidebar style="color:white;">
      <h2>Connect by Ameelio.</h2>
      <div class="container-fluid">
        <div class="row" style="margin:none;">
          <div class="col-lg-2">
            <img src="headphones.jpg">
          </div>
          <div class="col-lg-10" style="margin:none;">
            <p>Calling...</p>
            <p>User's Name</p>
            <p>address</p>
          </div>
        </div>
      </div>
      <h3>Home</h3>
      <ul class="sidebar-panel-nav">
        <li>
          <a href="#profile">Profile</a>
        </li>
        <li>
          <a href="#invite">Invite Friends</a>
        </li>
        <li>
          <a href="#settings">Settings</a>
        </li>
        <li>
          <a href="#help">Help Center</a>
        </li>
        <li>
          <a href="#team">Team Ameelio</a>
        </li>
      </ul>
    </Sidebar>
  </div>
</template>

<script>
import Burger from "./components/Menu/Burger.vue";
import Sidebar from "./components/Menu/Sidebar.vue";

export default {
  name: "app",
  components: {
    Burger,
    Sidebar
  }
};
</script>
<style>
html {
  height: 100%;
  overflow: hidden;
}

body {
  border: 0;
  margin: 0;
  padding: 0;
  font-family: "Lato";
  height: 100%;
  background: rgb(101, 31, 87);
  background-image: url("https://videohive.img.customer.envatousercontent.com/files/751ecf80-46c2-489a-8bae-95322ea403b5/inline_image_preview.jpg?auto=compress%2Cformat&fit=crop&crop=top&max-h=8000&max-w=590&s=69336bd36937a9656bd7efc97a2b0e37");
  background-repeat: no-repeat;
  background-size: cover;
}

.logo {
  align-self: center;
  color: rgb(0, 0, 0);
  font-weight: bold;
  font-family: "Lato";
}

.main-nav {
  display: flex;
  justify-content: center;
  padding: 0.5rem 3rem;
  bottom: 0;
  position: absolute;
  background: rgb(255, 255, 255);
  width: 100%;
}

ul.sidebar-panel-nav {
  list-style-type: none;
}

ul.sidebar-panel-nav > li > a {
  color: #fff;
  text-decoration: none;
  font-size: 1rem;
  display: block;
  padding-bottom: 0.5em;
}
.button {
  border: none;
  color: white;
  padding: 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 15px;
  border-radius: 50%;
}
</style>
