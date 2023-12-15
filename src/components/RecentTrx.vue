<script></script>

<template>
  <div class="card-container border">
    <div class="info-container">
      <div class="leftside-info">
        <div class="logo-container">
          <img src="../assets/grad-cap.png" alt="category logo" />
        </div>
        <div class="title-info">
          <h4 class="seller-name">Education</h4>
          <h5 class="gray">Brightwise</h5>
        </div>
      </div>
      <div class="rightside-outter">
        <div class="rightside-info">
          <h4 class="ammount-paid">$500</h4>
          <h5 class="gray">12-11-2023</h5>
        </div>
        <svg
          id="Arrow_Right_1_24"
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
              transform=" translate(-12.02, -12)"
              d="M 5.651 23.5 L 18.227 12.374 C 18.333944533046886 12.279108355046809 18.395150636583406 12.14297397466161 18.395150636583406 12 C 18.395150636583406 11.857026025338392 18.333944533046886 11.720891644953193 18.227 11.626000000000001 L 5.651 0.5"
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
  border-radius: 100%;
  margin-right: 10px;
  border: 3px solid #31c452;
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

.seller-name {
  font-weight: bold;
}

svg {
  width: 12px;
  height: 12px;
  margin: 0 6px 0 10px;
}

.rightside-outter {
  display: flex;
  justify-content: center;
  align-items: center;
}

.ammount-paid {
  font-weight: bold;
}
</style>
