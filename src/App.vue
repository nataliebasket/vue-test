<script>
import NavigationMenu from './components/NavigationMenu.vue'
import Catalog from './components/Catalog.vue'
import Filter from './components/Filter.vue'
import Cart from './components/Cart.vue'


export default {
  components: {
    NavigationMenu,
    Catalog,
    Filter,
    Cart
  },
}
</script>

<template>
  <div class="container">
    <NavigationMenu />
    <Catalog />
    <Filter />
    <!-- <Cart /> -->
  </div>

</template>

<style>
.container {
  max-width: 600px;
  margin: 0 auto;
  background-color: white;
  padding: 20px;
}

body {
  background-color: bisque;
  font-family: sans-serif;
}


</style>

