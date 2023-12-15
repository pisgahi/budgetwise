<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <nav>
    <div class="left-nav">
      <div class="logo-container">
        <img class="images" src="../assets/budgetwise-logo.png" alt="logo" />
        <h4>Budgetwise</h4>
      </div>
      <div class="navlinks-container">
        <div class="nav-links">
          <RouterLink to="/" class="selected-link">Home</RouterLink>
          <RouterLink to="/">Community</RouterLink>
          <RouterLink to="/">FAQs</RouterLink>
        </div>
      </div>
    </div>
    <div class="profile-container">
      <div class="img-container">
        <img
          class="images pfp"
          src="../assets/stock_pfp.jpeg"
          alt="profile image"
        />
      </div>
      <h4>John Doe</h4>
    </div>
  </nav>
</template>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 60px;
  border-bottom: 1px solid #dddddd;
}

.left-nav {
  display: flex;
  margin-left: 35px;
}

.logo-container {
  display: flex;
  align-items: center;
  margin-right: 150px;
  cursor: pointer;
}

.navlinks-container {
  width: 300px;
  display: flex;
  align-items: center;
}

a {
  text-decoration: none;
  margin-right: 35px;
  color: black;
}

.selected-link {
  border-bottom: 2px solid #5157bf;
}

.nav-links {
  height: 35px;
  display: flex;
  align-items: center;
}

.profile-container {
  display: flex;
  align-items: center;
  margin-right: 35px;
  cursor: pointer;
}

.img-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.images {
  width: 35px;
  margin-right: 6px;
}

.pfp {
  border-radius: 100%;
}
</style>
