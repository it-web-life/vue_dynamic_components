<template>
  <div class="block">
    <h2>これはHogeコンポーネントです</h2>
    <input type="text" v-model="text">
  </div>
</template>

<script>
export default {
  name: 'Hoge',
  data() {
    return {
      text: '',
    }
  },
  // ライフサイクル
  created() {
    console.log('created Hoge Component!!');
  },
  destroyed() {
    console.log('destroyed Hoge Component!!');
  },
  activated() {
    console.log('activated Hoge Component!!');
  },
  deactivated() {
    console.log('deactivated Hoge Component!!');
  },
}
</script>

<style scoped>
  .block {
    background-color: #fff;
    padding: 20px;
  }

  p {
    text-align: left;
  }
</style>
