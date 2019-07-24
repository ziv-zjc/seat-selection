<template>
  <div class="main-wrap">
    <div class="area-1" v-for="(seatNum, rowNum, index) in uiParam" v-bind:key="index">
      <div v-for="n in toInt(rowNum)" class="row" v-bind:key="n">
        <i v-for="m in (seatNum + rowNum)" class="iconfont icon-seat-default" v-bind:key="m"></i>
      </div>
    </div>
  </div>
</template>

<script>
function toInt(param) {
  return param - "0";
}

export default {
  // name: "home",

  components: {
    // HelloWorld,
  },

  data: function() {
    return {
      uiParam: {
        "50": 50
      }
    };
  },

  method: {},
  computed: {}
};
</script>

<style lang="scss">
// 线条总数

$total: 13;

// 每个线条相差的角度

$angel: 360/ ($total - 1);

.area-1 {
  // background: black;

  width: 400px;

  height: 400px;

  position: relative;

  i {
    position: absolute;

    display: block;

    width: 100%;

    height: 200px;

    top: 50%;

    transform-origin: 50% 50%;

    // &:before {
    //   display: block;

    //   content: "";

    //   height: 100%;

    //   width: 10%;

    //   // background: white;
    // }

    @for $i from 1 through $total {
      &:nth-child(#{$i}) {
        transform: rotate(#{$angel * ($i - 1)}deg);
      }
    }
  }
}
</style>