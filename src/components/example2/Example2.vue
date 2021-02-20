<template>
  <div class="wrap">
    <h3>keep-aliveを使ったインスタンスのキャッシュ</h3>
    <div class="tab-button">
      <button @click="current = 'Fuga'">Switch Fuga</button>
      <button @click="current = 'Hoge'">Switch Hoge</button>
    </div>
    <div class="tab-contents">
      <keep-alive>
        <comopnent :is="current"></comopnent>
      </keep-alive>
    </div>
  </div>
</template>

<script>
import Fuga from './Fuga.vue';
import Hoge from './Hoge.vue';

export default {
  name: 'Main',
  components: {
    Fuga,
    Hoge
  },
  data() {
    return {
      current: 'Fuga',
    }
  }
}
</script>

<style scoped>
.wrap {
  width: 100%;
  max-width: 500px;
  margin: 50px auto 100px;
}
.tab-button {
  text-align: center;
}
.tab-contents {
  border: 1px solid #dedede;
}
</style>
