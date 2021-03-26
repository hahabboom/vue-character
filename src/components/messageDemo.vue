<template>
  <div class="demo1">
    <div>{{msg2}}</div>
    <input type="text" :value="text" @input="$emit('change', $event.target.value)">
<!--    <input type="text" :value="text">-->
  </div>
<!--<div>-->
<!--&lt;!&ndash;  <input type="text" v-model="text">&ndash;&gt;-->
<!--</div>-->
</template>

<script>
export default {
  name: 'messageDemo',
  model: {
    prop: 'text',
    event: 'change'
  },
  data () {
    return {
    }
  },
  props: ['text', 'msg2'],
  watch: {},
  methods: {},
  computed: {},
  created () {
  },
  mounted () {
  }
}
</script>

<style scoped>
.demo1{
  display: flex;
  height: 90px;
  align-items: center;
  background-color: #E4C6BB;
}
.demo1Inner{
  height: 50px;
  display: flex;
  align-items: center;
  background-color: #9D8488;
}
</style>
