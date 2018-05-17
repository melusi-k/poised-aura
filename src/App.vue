<template>
      <div>
        <intro></intro>
        <div id="body">
          <div id="current">
            <current v-bind:currentCurrency="currentCurrency"></current>
          </div>
          <div id="previous">
            <previous v-bind:previousCurrency="previousCurrency"></previous>
          </div>
        </div>
      </div>
    </template>
    <script>
        import Intro from './components/Intro.vue';
        import Current from './components/Current.vue';
        import Previous from './components/Previous.vue';
        export default {
          name: 'app',
          components: {Intro, Current, Previous},
          data() {
            return {
              currentCurrency: {BTC: '', ETH: '', LTC: ''},
              previousCurrency: {
                yesterday: {}, twoDays: {}, threeDays: {}, fourDays: {}, fiveDays: {}
              }
            }
          },
          methods: {
            // Stub
          },
          created() {
            // Stub
          }
        }
        </script>
        <style>
    @import url('https://fonts.googleapis.com/css?family=Lato');
    * {
      margin : 0px;
      padding : 0px;
      font-family: 'Lato', sans-serif;
    }
    body { height: 100vh; width: 100%; }
    .row { display: flex; flex-wrap: wrap; }
    h1 { font-size: 48px; }
    a { color: #FFFFFF; text-decoration: none; }
    a:hover { color: #FFFFFF; }
    a:visited { color: #000000; }
    .button {
      margin: auto;
      width: 200px;
      height: 60px;
      border: 2px solid #E36F55;
      box-sizing: border-box;
      border-radius: 30px;
    }
    #body {
      max-width: 90%;
      margin: 0 auto;
      padding: 1.5em;
      text-align: center;
      color:rgb(0, 193, 131);
    }
    #current { padding: 2em 0em; }
    #previous { padding: 2em 0em; }
    </style>
