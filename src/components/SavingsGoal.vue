<script></script>

<template>
  <div class="snippet-container border">
    <div class="goal-title">
      Italy Trip <span class="see-details purple">See details</span>
    </div>
    <div class="budget-info">
      <div>
        <img src="../assets/goals-chart.jpg" alt="" />
      </div>

      <div class="stats">
        <h4>Total savings: $300 of $3,000 by April 15, 2023</h4>
      </div>
    </div>
  </div>
</template>

<style scoped>
.snippet-container {
  width: 380px;
  height: 200px;
  border-radius: 10px;
  border: 2px solid gra;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.budget-info {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100%;
  margin-bottom: 14px;
}

.stats {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 210px;
}

img {
  width: 130px;
  height: 130px;
  object-fit: contain;
  border-radius: 100%;
}

.goal-title {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 12px;
  width: 95%;
  font-weight: bold;
}

.see-details {
  font-size: 12px;
}
</style>
