<template>
  <div id="app">
    <div id="nav">
      <div class="nav-button">
        <router-link to="/welcome" class="nav-link">Home</router-link>
      </div>
      <div class="nav-button">
        <router-link to="/" class="nav-link">Cats</router-link>
      </div>
      <div class="nav-button">
        <router-link to="/donate" class="nav-link">Donate</router-link>
      </div>
    </div>
    <div id="menu">
      <router-view />
    </div>
    <div id="github-footer">
      Github: <a href="https://github.com/roundpigeon/creativeproject3">creativeproject3</a>
    </div>
  </div>
</template>

<style>
#nav {
  display: flex;
  justify-content: center;
  font-size: 2rem;
  width: 50%;
  margin-left: auto;
  margin-right: auto;
}

#menu {
  display: flex;
  justify-content: center;
}

#app {
  font-family: 'Noto Sans JP', sans-serif;
  border: 3px solid black;
  padding: 10px 10px 10px 10px;
  margin-left: auto;
  margin-right: auto;
  width: 80%;
}

.nav-link {
  text-decoration: none;
}

.nav-link:visited {
  color: black;
}

.nav-button {
  border: 2px solid black;
  margin: 10px 5px 10px 5px;
  padding: 0.5rem 1rem 0.5rem 1rem;
  border-radius: 5px;
}

.nav-button:hover {
  background-color: #e6e6e6;
}

#github-footer {
  display: flex;
  justify-content: center;
  margin: 2rem 0 2rem 0;
}
</style>
