<script setup lang="ts">
// import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
    
   <div id="app" style="height: 500px;">
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125"/>
    <HelloWorld msg="Vite + Vue3 + SSYUI" />
      <div style="margin-bottom: 20px;width: 200px;"> 
        <!-- <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav> -->
        <SButton>SButton</SButton><br>
        <SLink color="green" size="large">测试Link组件</SLink>
      </div> 
    <link rel="stylesheet" href="./stores/index.css" />
        <div style="margin-bottom:20px; width: 500px; height: 50px;">
            <SButton color="blue">主要按钮</SButton>
            <SButton color="green">绿色按钮</SButton>
            <SButton color="gray">灰色按钮</SButton>
            <SButton color="yellow">黄色按钮</SButton>
            <SButton color="red">红色按钮</SButton>
        </div>
      <br>
        <div style="margin-bottom:20px;  width: max-content; height: 50px;  margin-top: -80px;">
            <SButton color="blue" plain>朴素按钮</SButton>
            <SButton color="green" plain>绿色按钮</SButton>
            <SButton color="gray" plain>灰色按钮</SButton>
            <SButton color="yellow" plain>黄色按钮</SButton>
            <SButton color="red" plain>红色按钮</SButton>
        </div>
        <br>
        <div style="margin-bottom:20px;  width: max-content; height: 50px; margin-top: -90px;">
            <SButton size="small" plain>小按钮</SButton>
            <SButton size="medium" plain>中按钮</SButton>
            <SButton size="large" plain>大按钮</SButton>
        </div>
        <br>
        <div style="margin-bottom:20px;  width: max-content; height: 50px; margin-top: -80px;">
            <SButton color="blue" round plain icon="search">搜索按钮</SButton>
            <SButton color="green" round plain icon="edit">编辑按钮</SButton>
            <SButton color="gray" round plain icon="check">成功按钮</SButton>
            <SButton color="yellow" round plain icon="message">提示按钮</SButton>
            <SButton color="red" round plain icon="delete">删除按钮</SButton>
        </div>
        <br>
        <div style="margin-bottom:20px;  width: max-content; height: 50px; margin-top: -90px;">
            <SButton color="blue" round plain icon="search"></SButton>
            <SButton color="green" round plain icon="edit"></SButton>
            <SButton color="gray" round plain icon="check"></SButton>
            <SButton color="yellow" round plain icon="message"></SButton>
            <s-button color="red" round plain icon="delete"></s-button>
        </div>
      </div>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0; 
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

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  /* .logo {
    margin: 0 2rem 0 0;
  } */

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
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
