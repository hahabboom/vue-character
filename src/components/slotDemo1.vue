<template>
  <div class="demo2">
    <slot>{{msg}}</slot>
  </div>
</template>

<script>
export default {
  name: 'slotDemo1',
  data() {
    return {
      msg: '默认内容'
    }
  },
  props: {},
  watch: {},
  methods: {},
  computed: {},
  created() {
  },
  mounted() {
  }
}
</script>

<style scoped>
.demo2{
  height: 90px;
  background-color: #75AC47;
}
</style>
