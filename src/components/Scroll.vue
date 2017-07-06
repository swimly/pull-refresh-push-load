<template>
  <div class="scroll-view">
    <slot name="refresh"></slot>
    <div class="content" ref="content">
      <slot name="content"></slot>
    </div>
    <slot name="load">

    </slot>
  </div>
</template>
<script>
  import Iscroll from 'iscroll/build/iscroll-probe'
  export default {
    data () {
      return {
        options: {
          probeType: 1,
          mouseWheel: true,
          bounce: true,
          scrollY: false,
          scrollbars: false
        }
      }
    },
    mounted () {
      const myScroll = new Iscroll(this.$refs.content, this.options)
      myScroll.on('onScrollMove', this.onScroll)
      console.log(myScroll.options)
    },
    created () {
    },
    methods: {
      onScroll (e) {
        console.log(e)
      }
    }
  }
</script>
<style>
.scroll-view{overflow:hidden;height:100%;}
.content{overflow:auto;height:100%;}
</style>

