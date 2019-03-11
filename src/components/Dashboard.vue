<template>
  <div>
    <h1>{{title}}</h1>
    <div
      v-if="showTickets"
      style="border:red thin solid"
    >
      <h2>Tickets</h2>
      <ul>
        <li v-for="ticket in tickets">
          Id: {{ticket.Id}} Comment: {{ticket.Comments}} Created: {{ticket.DateCreated}}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Dashboard',
  data () {
    return {
      title: "Dashboard",
      showTickets: true,
      tickets: [
        { Id: '1', Comments: 'pc is slow', DateCreated: '03/11/2019 03:20' },
        { Id: '2', Comments: 'cannot login', DateCreated: '03/11/2019 05:20' },
        { Id: '3', Comments: 'powerchart crashsed', DateCreated: '03/11/2019 16:20' }
      ]
    }
  },
}
</script>

<style scoped>
</style>