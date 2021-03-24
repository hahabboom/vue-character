<template>
  <div class="demo2">
    <slot>{{msg}}</slot>
  </div>
</template>

<script>
export default {
  name: 'slotDemo1',
  data () {
    return {
      msg: '默认内容'
    }
  },
  props: {},
  watch: {},
  methods: {
  },
  computed: {},
  created () {
  },
  mounted () {
    let m = {}
    let name = 'hahabboom'
    Object.defineProperty(m, 'name', {
      get: function () {
        console.log('get', name)
        return name
      },
      set: function (newVal) {
        console.log('set', name)
        name = newVal
      }
    })
    console.log(m.name)
    m.name = 'lisa'
  }
}
</script>

<style scoped>
.demo2{
  height: 90px;
  background-color: #75AC47;
}
</style>
