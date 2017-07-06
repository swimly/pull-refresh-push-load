<template>
  <div id="app" class="app">
    <scroll>
      <div slot="content">
        <ul class="list">
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
          <li><a href="#">这是列表</a></li>
        </ul>
      </div>
    </scroll>
  </div>
</template>

<script>
import scroll from '@/components/Scroll'

export default {
  name: 'app',
  components: {
    scroll
  }
}
</script>

<style>
html{font-size:calc(3.75vw);height:100%;}
body{margin:0;height:100%;}
.app{height:100%;}
.list{list-style: none;padding:0;margin:0;}
.list a{display:block;font-size:1.4rem;color:#666;text-decoration:none;padding:0.8rem 1rem;border-bottom:1px dashed #ccc;}
</style>
