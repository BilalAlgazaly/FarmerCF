<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>
<template>
    <header>
          <div class="top-section">
            <div class="background-design"></div>
            <div class="logo-container">
                <img src="FClogo.png" alt="Logo" class="logo">
            </div>
          </div>
  </header>
    

  <body>
  <div class="wrapper">
    <nav>
      <!-- Hi hi -->
      <ul>g
     <li><a href="#">About Us</a></li>
      <li><a href="#">Contact Us</a></li>
      <li><a href="#">Login</a></li>
</ul>
    </nav>

    <div class="content">
      <div class="container">
        <div class="left-panel">
          <!-- Left panel content -->
        </div>
        <div class="right-panel">
          <h1>HelloWorld</h1>
          <!-- Right panel content -->
        </div>
      </div>
    </div>
  </div>
</body>

</template>



<style>
.top-section {
  position: relative;
}
.background-design {
  position: absolute;
  top: 0;
  right: 100%;
  left: -300%;
  width: 750%;
  height: 100%;
  background-image: linear-gradient(to bottom right,#ff3b3b ,#32a852 );
  
}
.logo-container {
  margin-bottom: 400%;
 right: -100px;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 26vh;
  
  
  
  
}

.logo {
  max-width: 100%;
  max-height: 100%;
  
}




nav {
  background-color: #3a3a3a;
  height: 50px;
  margin: 0 auto;
  right: -100px;
  left: -60%;
  margin-top: 200px;
  width: 100%;
  max-width: 960px; /* adjust this value based on your design */
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li {
  float: left;
}

a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

a:hover {
  background-color: #111;
}

</style>









  <RouterView />


<style scoped>
.container {
  display: flex;
  flex-direction: column;
  height: 100vh;
}


.left-panel {
  flex: -1;
  background-color:rgb(59, 42, 42); /* Change this to your desired background color */
  width: 100%;
  float: left;
}

.right-panel {
  flex: 1;
  background-color:blue ; /* Change this to your desired background color */
  width: 500%;
  float: right;}
/*header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

/*@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}*/
</style>
