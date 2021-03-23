<template>
  <div class="main">
    <h2>Vue2.x特性总结</h2>
    <ul>
      <li>1. v-model双向绑定</li>
      <li>{{name}}</li>
      <li><message-demo v-model="name"></message-demo></li>
      <li>2. slot</li>
      <li><slot-demo1>{{slotMsg}}</slot-demo1></li>
      <li><slot-demo2 v-slot:slotData></slot-demo2></li>
    </ul>
  </div>
</template>

<script>
import MessageDemo from "./messageDemo";
import SlotDemo1 from "./slotDemo1";
import SlotDemo2 from "./slotDemo2";
export default {
  name: 'mainBody',
  components: { SlotDemo2, SlotDemo1, MessageDemo },
  data () {
    return {
      name: '123',
      slotMsg: '我要挤掉你！',
      slotData: '挤掉你第二次'
    }
  },
  props: {},
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
.main{
  height: 100%;
  width: 100%;
  background-color: #A0B574;
}
</style>
