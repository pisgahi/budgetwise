<script>
export default {
  data() {
    return {
      progress: 40,
    };
  },
  methods: {
    makeProgress() {
      if (this.progress < 100) {
        this.progress += 5;
      }
    },
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
  <div class="card-container">
    <div class="info-container">
      <div class="leftside-info">
        <div class="logo-container">
          <img src="../assets/grad-cap.png" alt="category logo" />
        </div>
        <div class="title-info">
          <h4 class="purchase-category">Education</h4>
          <h5>spent <span class="green-text">$40</span> of $100</h5>
        </div>
      </div>
      <div class="rightside-info">
        <h4 class="green-text">$60</h4>
        <h4>left</h4>
      </div>
    </div>
    <div id="progress-bar">
      <div class="holder">
        <div class="bar" :style="{ width: progress + '%' }">
          <span class="progress-span">${{ progress }}</span>
        </div>
      </div>
      <button @click="makeProgress">+</button>
    </div>
  </div>
</template>

<style scoped>
.card-container {
  width: 645px;
  padding: 6px;
  border-bottom: 1px solid gray;
  margin-bottom: 14px;
}

.info-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.leftside-info {
  display: flex;
  align-items: center;
}

img {
  width: 30px;
  height: 30px;
  border-radius: 100%;
  margin-right: 10px;
}

.rightside-info {
  display: flex;
  flex-direction: column;
  align-items: end;
}

.status-bar-container {
  width: 645px;
  display: flex;
  justify-content: center;
}

.purchase-category {
  font-weight: bold;
}

/* PROGRESS STYLING */

#progress-bar {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  height: 20px;
}

.holder {
  height: 15px;
  width: 580px;
  border: 1px solid #aaa;
  /* padding: 3px; */
  /* background-color: yellow; */
  display: flex;
  align-items: center;
  justify-content: start;
}

.bar {
  background: #46bdc6;
  height: 15px;
  width: 15px;
  display: flex;
  align-items: center;
  justify-content: end;
}
.progress-span {
  float: right;
  /* padding: 4px; */
  color: #fff;
  font-size: 12px;
}

button {
  margin: 10px;
  border: 1px solid #aaa;
  background: none;
  border-radius: 50%;
  /* padding: 5px 8px; */
  outline: none;
  cursor: pointer;
}
</style>
