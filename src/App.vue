<script lang="ts">
export default {
  data() {
    return {
      name: 'Charis Ginn',
      status: 'inactive',
      list: ['item 1', 'item 2', 'item 3'],
    }
  },
}
</script>

<template>
  <h1>Hi there</h1>
  <p v-if="status == 'active'">User is active</p>
  <p v-else-if="status === 'pending'">User is pending</p>
  <p v-else>User is not active</p>

  <h2>Items</h2>
  <ul>
    <li v-for="item in list" :key="item">{{ item }}</li>
  </ul>
</template>
