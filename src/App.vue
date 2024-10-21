<template lang="pug">
  div(id="app")
    Navbar
    b-container.mt-2
      b-row
        b-col 
          Stat
      b-row
        b-col
          PoolTable.mt-2

</template>

<script>
import Navbar from '@/components/navbar.vue'
import Stat from '@/components/stat.vue'
import PoolTable from '@/components/pool-table.vue'
export default {
  name: 'App',
  components: {
    Navbar,
    Stat,
    PoolTable
  }
}
</script>

<style>

</style>
