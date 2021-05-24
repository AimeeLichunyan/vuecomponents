<template>
  <div id="app">
    <div id="nav">
      <!-- 普通按钮 -->
     <aimee-button>默认按钮</aimee-button>
     <aimee-button type="primary">主要按钮</aimee-button>
     <aimee-button type="warning">警告按钮</aimee-button>
     <aimee-button type="danger">危险按钮</aimee-button>
     <aimee-button type="success">成功按钮</aimee-button>
      <br>
      <!-- 带icon的按钮 -->
     <aimee-button type="info" icon="sousuo">信息按钮</aimee-button>
     <aimee-button type="info" icon="sousuo" icon-position="right">信息按钮</aimee-button>
     <aimee-button type="info" loading icon="edit">信息按钮</aimee-button>
     <br>
     <!-- 事件button -->
    <aimee-button type="info" @click="fn">触发事件</aimee-button>
    <br>
    <!-- 组合button -->
    <div class="style-class"></div>
    <aimee-group-button>
      <aimee-button type="primary" icon="left" icon-position="left">上一页</aimee-button>
      <aimee-button type="primary" icon="right" icon-position="right">下一页</aimee-button>
    </aimee-group-button>
     <br>
     <aimee-icon icon="sousuo"></aimee-icon>
     <aimee-icon icon="edit"></aimee-icon>
    </div>
  </div>
</template>
<script>
export default {
  name: 'App',
  methods: {
    fn(e) {
      console.log(e)
    }
  }
}
</script>
<style lang="scss">
  .style-class {
    margin: 10px 0;
  }
</style>
