<script></script>

<template>
  <div class="card-container border">
    <div class="info-container">
      <div class="leftside-info">
        <div class="logo-container">
          <img src="../assets/boa.png" alt="category logo" />
        </div>
        <div class="title-info">
          <h5 class="bank-name">Bank of America</h5>
          <div class="gray">...4765</div>
        </div>
      </div>

      <div class="rightside-outter">
        <div class="rightside-info">
          <h5 class="purple">Balance</h5>
          <h3 class="purple">$1,326.23</h3>
        </div>
        <svg
          id="Arrow_Up_1_24"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
        >
          <rect
            width="24"
            height="24"
            stroke="none"
            fill="#000000"
            opacity="0"
          />

          <g transform="matrix(0.87 0 0 0.87 12 12)">
            <path
              style="
                stroke: rgb(0, 0, 0);
                stroke-width: 1;
                stroke-dasharray: none;
                stroke-linecap: round;
                stroke-dashoffset: 0;
                stroke-linejoin: round;
                stroke-miterlimit: 4;
                fill: none;
                fill-rule: nonzero;
                opacity: 1;
              "
              transform=" translate(-12.04, -12)"
              d="M 23.535 18.373 L 12.409 5.8 C 12.314095536193784 5.692715571505556 12.177736887175492 5.631284998151139 12.034500000000001 5.631284998151139 C 11.891263112824507 5.631284998151139 11.754904463806216 5.692715571505556 11.66 5.8 L 0.535 18.373"
              stroke-linecap="round"
            />
          </g>
        </svg>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card-container {
  padding: 4px;
  border-radius: 10px;
  margin-bottom: 8px;
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

.logo-container {
  display: flex;
  justify-content: center;
  align-items: center;
}

img {
  width: 30px;
  height: 30px;
  border-radius: 10px;
  margin-right: 10px;
}

.rightside-outter {
  display: flex;
  justify-content: center;
  align-items: center;
}

svg {
  width: 12px;
  height: 12px;
  margin: 0 6px 0 10px;
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

.bank-name {
  font-weight: bold;
}
</style>
