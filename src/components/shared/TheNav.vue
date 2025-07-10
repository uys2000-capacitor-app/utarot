<template>
  <ul class="menu w-full" :class="{ 'menu-horizontal': horizontal }">
    <!-- Navbar menu content here -->
    <li><a>Anasayfa</a></li>
    <li><a>Hakkımda</a></li>
  </ul>
</template>

<script lang="ts">
export default {
  props: {
    horizontal: {
      type: Boolean,
      default: false
    }
  }
}
</script>
<style>body {
  background-color: #1f1b24; 
}
</style>