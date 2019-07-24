<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>-->
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
@font-face {
  font-family: "iconfont";
  src: url("assets/fonts/iconfont.eot?t=1563973837110"); /* IE9 */
  src: url("assets/fonts/iconfont.eot?t=1563973837110#iefix")
      format("embedded-opentype"),
    /* IE6-IE8 */
      url("data:application/x-font-woff2;charset=utf-8;base64,d09GMgABAAAAAALoAAsAAAAABrwAAAKbAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAHEIGVgCCcAqBSIFAATYCJAMICwYABCAFhG0HMBvmBRHVk19kXx5wh+kW3gHhbdBS5/ijVPwpNYyLiFnFQb8Pnn/HXu9LUgDgEam6TiHi8YAs7H5jmGnW08nZQX+BbwlcPOKAAsAIS1LU/4yBhQ4A33ez6hoVocqQ2Fv+tmX8wE5fGm4cXFM/Ni+QPKC5ZQRHAg5sOsAujCTZQAbgG8YucAnHIYA9wSQildWNndhisMYJILOmTx2Pbc6LwbCELYJ1zVKDrMEKW7VU3YXV4fflT7rYgsJKY5W0TqmaROn3zE7RcyzDoI/gAwGttgI0kAgYkM7aaDMaYVSNfdQQDvsqFPheln09stc/D7HGyncEIBBy74nn8m81XwFg4u5yoHbUIlDxjNkzp2XH/MUx3Chif+h5sN5+O8bh4E0/5YIetOPp8IUDcZRdj7M3HfKU3U9yXC4+CmKTvD2hU911z7es3YPb3Kf71M+HmtB17r1zfPh2DjMMkh4e77xxVWhFzYTF7XD6f++0Y88cmbc2aOWZ8DM7ndaOCqUAWDYb9PS/+RtKr0kecSnc1sEA8KrH7iF+PzvYntMm8O94PZuMLrB0yqi8WruifNRYBdhjD1jATnfej1V63ahZsM3xGChsCAKNLZGoISaCFQ5kgjW2lIA9CdSsdsCDUTRi7IB4FgIQXDkNCmdug8aVe6ghvgMrvPkH1riKBnu6xWNLB6KFGX0UtaGj5k9jKxs7BvNR4RX9vtSaFYS0JzSNASpCXkxcsEHnmJE+fWnGxCorncFpWBahqDKhtTCYxSrLuO5JoZXVeaKoDR01fxpb2djvbL70+Sv6fam1pazG/oSmsXcqQt4DvUi3XmX3ck769KUZE6usdAZmLHZUKNYPmtBaGEaEY5WhdtxXGtaXrx+Qw6qwVErsfhrM3uWL0TkA")
      format("woff2"),
    url("assets/fonts/iconfont.woff?t=1563973837110") format("woff"),
    url("assets/fonts/iconfont.ttf?t=1563973837110") format("truetype"),
    /* chrome, firefox, opera, Safari, Android, iOS 4.2+ */
      url("assets/fonts/iconfont.svg?t=1563973837110#iconfont") format("svg"); /* iOS 4.1- */
}

.iconfont {
  font-family: "iconfont" !important;
  font-size: 12px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-seat-default:before {
  content: "\e62f";
}
</style>
