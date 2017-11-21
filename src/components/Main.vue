<template>
  <div>
      <h2>我是子组件的标题</h2>
      <div>
        <slot name="header">这是默认header</slot>
      </div>
       <div>
        <slot name="footer">这是默认footer</slot>
      </div>     
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name:"main",

})
</script>
