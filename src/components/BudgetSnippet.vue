<script>
export default {
  data() {
    return {
      progress: 80,
    };
  },
  components: {
    Progressbar: {
      template: `
        <div id="progress-bar">
          <div class="holder">
            <div class="bar" :style="{ width: progress + '%' }">
              <span>{{ progress }}%</span>
            </div>
          </div>
          <button @click="makeProgress">+</button>
        </div>
      `,
      props: ["progress"],
      methods: {
        makeProgress() {
          this.$emit("makeProgress");
        },
      },
    },
  },
};
</script>

<template>
  <div class="snippet-container border">
    <div class="budget-info">
      <div class="stats">
        <h5 class="gray snap-title">Spent</h5>
        <h2 class="spent">$800</h2>
      </div>

      <div class="stats middle-stat">
        <h5 class="gray snap-title">Available</h5>
        <h2 class="green-text">$1200</h2>
      </div>

      <div class="stats">
        <h5 class="gray snap-title">Budget</h5>
        <h2>$2000</h2>
      </div>
    </div>
    <div class="progress-bar">
      <div id="progress-bar">
        <div class="holder">
          <div class="bar" :style="{ width: progress + '%' }"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.snippet-container {
  width: 380px;
  height: 120px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 14px;
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
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 120px;
}

.middle-stat {
  border-left: 2px solid #dddddd;
  border-right: 2px solid #dddddd;
}

.snap-title {
  font-weight: bold;
}

.spent {
  color: #fb5c5d;
}

/* PROGRESS STYLING */

#progress-bar {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  border-radius: 6px;
}

.holder {
  height: 20px;
  width: 360px;
  border: 1px solid #aaa;
  display: flex;
  align-items: center;
  justify-content: start;
  border-radius: 6px;
}

.bar {
  background: #5157bf;
  height: 20px;
  width: 15px;
  border-radius: 6px;
}
</style>
