<template>
  <div>
    <nav>
      <h1><NuxtLink to="/"><span>Royal Dev</span></NuxtLink></h1>
      <ul>
        <li><NuxtLink to="/rust"><span>Rust</span></NuxtLink></li>
        <li><NuxtLink to="/java"><span>Java</span></NuxtLink></li>
        <li><NuxtLink to="/springboot"><span>Springboot</span></NuxtLink></li>
        <li><NuxtLink to="/javascript"><span>Javascript</span></NuxtLink></li>
        <li><NuxtLink to="/vue"><span>Vue</span></NuxtLink></li>
        <li><NuxtLink to="/react"><span>React</span></NuxtLink></li>
      </ul>
      <h2>&#8659;</h2>
    </nav>
    <div class="main-container">
      <NuxtPage />
    </div>
  </div>
</template>
<style>
*,
body {
  box-sizing: border-box;
  margin: 0;
}
</style>
<style scoped>
.main-container {
  padding: 2% 14% 0;
  line-height: 2em;
}
nav {
  background-color: rgb(51, 51, 199);
  color: white;
  height: 6em;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 14%;
}

nav ul li span, nav h1 span {
  color: white;
}
nav ul li:hover span, nav h1:hover span  {
  color: rgb(207, 89, 89);
  text-decoration: underline;
}
nav h2 {
  display: none;
}

@media only screen and (max-width: 876px) {
  .main-container {
    padding: 2% 2% 0;
  }
  nav {
    padding: 0 2%;
  }
}
@media only screen and (max-width: 680px){
	nav ul {
    visibility: hidden;
  }
  nav h1 {
    width: 100%;
  }
  nav h2 {
    display: block;
    font-size: 3em;
    padding-right: 0.4em;
  }
}

nav ul {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

nav ul li {
  list-style: none;
  padding-left: 1em;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande',
    'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  font-size: 1.2em;
}
</style>
