<template>
  <div class="wrap">
    <h3>componentタグとis属性によるコンポーネントの動的切り替え</h3>
    <div class="tab-button">
      <button @click="current = 'Foo'">Switch Foo</button>
      <button @click="current = 'Bar'">Switch Bar</button>
    </div>
    <div class="tab-contents">
      <comopnent :is="current"></comopnent>
    </div>
  </div>
</template>

<script>
import Foo from './Foo.vue';
import Bar from './Bar.vue';

export default {
  name: 'Main',
  components: {
    Foo,
    Bar
  },
  data() {
    return {
      current: 'Foo',
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
