<script setup>
import { RouterLink, RouterView } from 'vue-router'


</script>

<template>

  <header>
    <nav>
        
      </nav>
      <nav class="desktop-nav">
        <div class="logo">Hardy</div>
        <div>
            <ul class="navlinks">
                <li><RouterLink class="Link" to="/">Home</RouterLink></li>
                <li><RouterLink class="Link" to="/about">Portfolio</RouterLink></li>
                <li><RouterLink class="Link" to="/contact">Contact</RouterLink></li>
                <li><div class="flex">
        <div class="mode-toggle" @click="modeToggle" :class="darkDark">
            <div class="toggle">
                <div id="dark-mode" type="checkbox"></div>
            </div>
        </div>
    </div></li>
            </ul>
        </div>
    </nav>
  </header>
  <RouterView />
</template>

<style scoped>
li{
  color:black;
  text-decoration: none;
}

.prof{
  display: flex;
  width: 420px;
  height: 600px;
}

.Link{
  color: black;
}
</style>
