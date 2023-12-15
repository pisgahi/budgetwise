<script setup></script>

<template>
  <div class="sidebar-container">
    <div class="sidebar-links">
      <RouterLink class="base-select" to="/">Overview</RouterLink>
      <RouterLink to="/">Budget</RouterLink>
      <RouterLink to="/">Transactions</RouterLink>
      <RouterLink to="/">Trends</RouterLink>
      <RouterLink to="/">Savings Goal</RouterLink>
      <RouterLink to="/">Alerts</RouterLink>
    </div>
  </div>
</template>

<style scoped>
.sidebar-container {
  width: 250px;
  height: 100vh;
  overflow: none;
  display: flex;
  flex-direction: column;
  align-items: center;
  border-right: 1px solid #dddddd;
}

.sidebar-links {
  width: 200px;
  height: 270px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-top: 20px;
}

a {
  text-decoration: none;
  height: 40px;
  display: flex;
  align-items: center;
  padding-left: 8px;
  color: black;
}

.base-select {
  border-left: 3px solid black;
}

a:active {
  border-left: 3px solid black;
}
</style>
