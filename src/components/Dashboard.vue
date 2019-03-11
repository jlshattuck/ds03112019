<template>
  <div>
    <h1>{{title}}</h1>
    <div v-if="showTickets" style="border:red thin solid">
        <h2>Tickets</h2>

    </div>
  </div>
</template>

<script>
export default {
  name: 'Dashboard',
  data () {
    return {
      title: "Dashboard",
      showTickets:true
    }
  },
}
</script>

<style scoped>
</style>