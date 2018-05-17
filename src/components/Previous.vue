<template>
      <div>
        <h2>Previous prices of coins</h2>
        <div id="first">
          <h2>Date:   {{previousCurrency.yesterday.DATE}}</h2>
          <p><label>1 BTC:</label> {{previousCurrency.yesterday.BTC}}</p>
          <p><label>1 ETH:</label> {{previousCurrency.yesterday.ETH}}</p>
          <p><label>1 LTC:</label> {{previousCurrency.yesterday.LTC}}</p>
        </div>
        <div id="second">
          <h2>Date:   {{previousCurrency.twoDays.DATE}}</h2>
          <p><label>1 BTC:</label> {{previousCurrency.twoDays.BTC}}</p>
          <p><label>1 ETH:</label> {{previousCurrency.twoDays.ETH}}</p>
          <p><label>1 LTC:</label> {{previousCurrency.twoDays.LTC}}</p>
        </div>
        <div id="third">
          <h2>Date:   {{previousCurrency.threeDays.DATE}}</h2>
          <p><label>1 BTC:</label> {{previousCurrency.threeDays.BTC}}</p>
          <p><label>1 ETH:</label> {{previousCurrency.threeDays.ETH}}</p>
          <p><label>1 LTC:</label> {{previousCurrency.threeDays.LTC}}</p>
        </div>
        <div id="fourth">
          <h2>Date:   {{previousCurrency.fourDays.DATE}}</h2>
          <p><label>1 BTC:</label> {{previousCurrency.fourDays.BTC}}</p>
          <p><label>1 ETH:</label> {{previousCurrency.fourDays.ETH}}</p>
          <p><label>1 LTC:</label> {{previousCurrency.fourDays.LTC}}</p>
        </div>
        <div id="fifth">
          <h2>Date:   {{previousCurrency.fiveDays.DATE}}</h2>
          <p><label>1 BTC:</label> {{previousCurrency.fiveDays.BTC}}</p>
          <p><label>1 ETH:</label> {{previousCurrency.fiveDays.ETH}}</p>
          <p><label>1 LTC:</label> {{previousCurrency.fiveDays.LTC}}</p>
        </div>
      </div>
    </template>
    <script>
        export default {
          name: 'app',
          props: {
            previousCurrency: { type: Object }
          },
          data () {
            return {}
          }
        }
        </script>
        <style scoped>
    #first, #second, #third, #fourth, #fifth {
      border: 1px solid #F5CE00;
      padding: 2em 0em;
      max-width: 90%;
      margin: 3px auto;
    }
    #first p, #second p, #third p, #fourth p, #fifth p {
      display: inline-block;
      padding: 0em 1.5em;
      font-size: 1.5rem;
    }
    h2 { font-size: 1.5em; }
    </style>
