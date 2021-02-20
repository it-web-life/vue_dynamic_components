<template>
  <div class="block">
    <h2>This is Fuga Component.</h2>
    <input type="text" v-model="text">
  </div>
</template>

<script>
export default {
  name: 'Fuga',
  data() {
    return {
      text: '',
    }
  },
  created() {
    console.log('created Fuga Component!!');
  },
  destroyed() {
    console.log('destroyed Fuga Component!!');
  },
  activated() {
    console.log('activated Fuga Component!!');
  },
  deactivated() {
    console.log('deactivated Fuga Component!!');
  },
}
</script>

<style scoped>
  .block {
    background-color: #dedede;
    padding: 20px;
  }
  
  p {
    text-align: left;
  }
</style>
