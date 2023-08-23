<!--
 * @Author: 姚恒锋 1921934563@qq.com
 * @Date: 2023-08-22 18:22:07
 * @LastEditors: 姚恒锋 1921934563@qq.com
 * @LastEditTime: 2023-08-23 12:00:59
 * @FilePath: \draggable-resizable-rotable\src\App.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <div id="app">
    <div style="height: 500px; width: 500px; border: 1px solid red; position: relative;">
      <vue-draggable-resizable :w="400" :h="400" :parent="true" :min-width="10" :min-height="20" :has-rotation="false">
        <p>旋转</p>
      </vue-draggable-resizable>
    </div>
  </div>
</template>

<script>
import VueDraggableResizable from './components/vue-draggable-resizable'
import './components/vue-draggable-resizable.css'

export default {
  name: 'app',
  components: {
    VueDraggableResizable
  }
}
</script>

<style>
  .vdr {
    border: 1px dashed black;
  }
</style>
