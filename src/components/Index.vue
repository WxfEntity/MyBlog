<template>
  <Row>
    <i-col span="11">
      <Card>
        <p slot="title">标准卡片</p>
        <p>卡片内容</p>
        <p>卡片内容</p>
        <p>卡片内容</p>
      </Card>
    </i-col>
    <i-col span="11" offset="2">
      <Card dis-hover>
        <p slot="title">禁用悬停阴影的卡片</p>
        <p>卡片内容</p>
        <p>卡片内容</p>
        <p>卡片内容</p>
      </Card>
    </i-col>
  </Row>
</template>
<script>
    export default {

    }
</script>

<style scoped>

</style>
