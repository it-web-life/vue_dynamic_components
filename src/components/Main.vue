<template>
  <div>
    <Example1></Example1>
    <Example2></Example2>
  </div>
</template>

<script>
import Example1 from './example1/Example1.vue';
import Example2 from './example2/Example2.vue';

export default {
  name: 'Main',
  components: {
    Example1,
    Example2
  },
  props: {
    msg: String
  },
  data() {
    return {
      current: 'Foo',
    }
  }
}
</script>
