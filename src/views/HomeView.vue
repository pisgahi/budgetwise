<script setup>
import SideBar from "../components/SideBar.vue";
import TrxCard from "../components/TrxCard.vue";
import BudgetSnippet from "../components/BudgetSnippet.vue";
import RecentTrx from "../components/RecentTrx.vue";
import BankBalance from "../components/BankBalance.vue";
import SavingsGoal from "../components/SavingsGoal.vue";
import SpendSnapshot from "../components/SpendSnapshot.vue";
</script>

<template>
  <main class="home-page-container">
    <div>
      <SideBar />
    </div>

    <div class="mid-section-container">
      <div class="budget-actions">
        <div class="budget-date-range">
          <div class="date-container">
            <select class="base-selector" name="dates" id="dates-selector">
              <option value="Weekly">Weekly Budget</option>
              <option value="Monthly">Monthly Budget</option>
              <option value="Yearly">Yearly Budget</option>
            </select>
          </div>
          <div class="specific-dates-selector">
            <select
              class="specific-selector green-text"
              name="dates"
              id="dates-selector"
            >
              <option value="Weekly">January 2023</option>
              <option value="Monthly">Febraury 2023</option>
              <option value="Yearly">March 2023</option>
              <option value="Weekly">April 2023</option>
              <option value="Monthly">May 2023</option>
              <option value="Yearly">June 2023</option>
              <option value="Weekly">July 2023</option>
              <option value="Monthly">August 2023</option>
              <option value="Yearly">Septemebr 2023</option>
              <option value="Weekly">October 2023</option>
              <option value="Monthly">Novemebr 2023</option>
              <option value="Yearly">Decemebr 2023</option>
            </select>
          </div>
        </div>
        <div class="budget-functioanlities">
          <svg
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

            <g transform="matrix(0.83 0 0 0.83 12 12)">
              <path
                style="
                  stroke: none;
                  stroke-width: 1;
                  stroke-dasharray: none;
                  stroke-linecap: butt;
                  stroke-dashoffset: 0;
                  stroke-linejoin: miter;
                  stroke-miterlimit: 4;
                  fill: rgb(0, 0, 0);
                  fill-rule: nonzero;
                  opacity: 1;
                "
                transform=" translate(-15, -15)"
                d="M 23 3 C 20.790861000676827 3 19 4.790861000676826 19 7 C 19.001782866247694 7.281166357331076 19.033206577012333 7.561361111649108 19.09375 7.8359375 L 10.011719 12.376953 C 9.253866777438894 11.504445134647924 8.155683524287866 11.002357547799328 7.000000000000002 11 C 4.790861000676826 11 3 12.790861000676827 3 15 C 3 17.209138999323173 4.790861000676826 19 7 19 C 8.156055212198664 18.998698187755465 9.255011018954107 18.497295170343904 10.013672 17.625 L 19.089844 22.164062 C 19.03061381338721 22.4387782327156 19.00049950956681 22.718971577925238 19 23 C 19 25.209138999323173 20.790861000676827 27 23 27 C 25.209138999323173 27 27 25.209138999323173 27 23 C 27 20.790861000676827 25.209138999323173 19 23 19 C 21.843944787801338 19.001301812244538 20.744988981045893 19.502704829656096 19.986328 20.375 L 10.910156 15.835938 C 10.969386186612791 15.5612217672844 10.999500490433189 15.281028422074762 11 14.999999999999998 C 10.998080050222471 14.719487064074768 10.96665714476816 14.43995425999575 10.90625 14.166015999999999 L 19.988281 9.625 C 20.746494206769245 10.496781890462847 21.844626705286966 10.998134169829504 23 11 C 25.209138999323173 11 27 9.209138999323173 27 7 C 27 4.790861000676826 25.209138999323173 3 23 3 z"
                stroke-linecap="round"
              />
            </g>
          </svg>

          <svg
            id="Setting_Menu_Vertical_24"
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

            <g transform="matrix(1.43 0 0 1.43 12 12)">
              <g style="">
                <g transform="matrix(1 0 0 1 0.02 -4.72)">
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
                    transform=" translate(-7.02, -2.28)"
                    d="M 5.52368 2.28125 C 5.52368 3.24125 6.06368 3.78125 7.02368 3.78125 C 7.98368 3.78125 8.52368 3.24125 8.52368 2.28125 C 8.52368 1.32125 7.98368 0.78125 7.02368 0.78125 C 6.06368 0.78125 5.52368 1.32125 5.52368 2.28125 Z"
                    stroke-linecap="round"
                  />
                </g>
                <g transform="matrix(1 0 0 1 0.02 0)">
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
                    transform=" translate(-7.02, -7)"
                    d="M 5.52368 7 C 5.52368 7.96 6.06368 8.5 7.02368 8.5 C 7.98368 8.5 8.52368 7.96 8.52368 7 C 8.52368 6.04 7.98368 5.5 7.02368 5.5 C 6.06368 5.5 5.52368 6.04 5.52368 7 Z"
                    stroke-linecap="round"
                  />
                </g>
                <g transform="matrix(1 0 0 1 0.02 4.72)">
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
                    transform=" translate(-7.02, -11.72)"
                    d="M 5.52368 11.7187 C 5.52368 12.6787 6.06368 13.2187 7.02368 13.2187 C 7.98368 13.2187 8.52368 12.6788 8.52368 11.7188 C 8.52368 10.7587 7.98368 10.2187 7.02368 10.2187 C 6.06368 10.2187 5.52368 10.7587 5.52368 11.7187 Z"
                    stroke-linecap="round"
                  />
                </g>
              </g>
            </g>
          </svg>
          <div class="add">+</div>
        </div>
      </div>

      <div class="trx-overview">
        <div class="trx-list">
          <h1 class="title">Categories</h1>
          <!-- Instead of mapping the component dynamically, I chose
        to reuse it with the same data to simplify the process, 
        and remove dependencey from mock data. -->
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
          <TrxCard />
        </div>
      </div>
    </div>

    <div class="right-side-container">
      <div class="right-section-container">
        <div class="snippet-container">
          <BudgetSnippet />
        </div>
        <div class="snapshot-container">
          <h1 class="recent-title">6 Month Snapshot</h1>
          <SpendSnapshot />
        </div>
        <div class="recent-trx-section">
          <h1 class="recent-title">
            Recent Transactions<span class="recent-all gray">See all</span>
          </h1>
          <RecentTrx />
          <RecentTrx />
          <RecentTrx />
          <RecentTrx />
        </div>
        <div class="balance-container">
          <h1 class="recent-title">Banks &amp; Credit Cards</h1>
          <BankBalance />
        </div>
        <div class="balance-container">
          <h1 class="recent-title">Savings Goals<span>+</span></h1>
          <SavingsGoal />
        </div>
      </div>
    </div>
  </main>
</template>

<style sscoped>
.snippet-container,
.snapshot-container,
.recent-trx-section,
.balance-container,
.balance-container {
  margin-bottom: 25px;
}

.home-page-container {
  display: flex;
  width: 100vw;
  justify-content: center;
  position: fixed;
  overflow: hidden;
}

.mid-section-container {
  width: 735px;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100vh;
  overflow-y: auto;
}

.budget-actions {
  width: 645px;
  height: 80px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 12px 0;
}

.budget-date-range {
  height: 55px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 4px;
}

.base-selector {
  font-size: 20px;
  font-weight: 700;
  background: transparent;
  border: none;
  margin-bottom: 4px;
  outline: none;
}

.specific-selector {
  font-size: 15px;
  height: 25px;
  border-radius: 8px;
  outline: none;
  background-color: #e6f5ea;
}

.specific-dates-selector {
  height: 40px;
}

select {
  cursor: pointer;
}

.budget-functioanlities {
  width: 120px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

svg {
  width: 25px;
  height: 25px;
  cursor: pointer;
}

.add {
  width: 40px;
  height: 40px;
  font-size: 20px;
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #5157bf;
  color: white;
  border-radius: 100%;
  padding-bottom: 4px;
}

.add-trx {
  width: 40px;
  height: 40px;
}

.right-side-container {
  width: 410px;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  height: 100vh;
  overflow: hidden;
}

.right-section-container {
  height: 100vh;
  overflow-y: auto;
}

.trx-overview {
  display: flex;
  flex-direction: column;
}

.trx-list {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.title {
  width: 645px;
  display: flex;
  justify-content: start;
  font-size: 15px;
  padding-left: 4px;
  font-weight: bold;
  margin: 6px;
}

.recent-title {
  display: flex;
  justify-content: space-between;
  font-size: 15px;
  padding-left: 4px;
  font-weight: bold;
  margin: 6px;
  margin-bottom: 8px;
}

.recent-all {
  font-size: 14px;
  display: flex;
  align-items: center;
}
</style>
