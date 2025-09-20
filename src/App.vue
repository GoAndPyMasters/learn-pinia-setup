

<template>
  <div class="app">
  <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  <RouterView />
</template>

<style>
.app {
text-align: center;
text-emphasis-color: #3434fa;
}
</style>
