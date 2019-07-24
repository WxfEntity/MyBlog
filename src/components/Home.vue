<template>
  <div >
      <Preview id="pre">
      </Preview>
    <Page id="page">
    </Page>
    <div>
    </div>
  </div>
</template>

<script>
  import Preview from './Preview.vue';
  import Page from './Page.vue';

  export default {
      components: {Preview,Page},
      name: "Home"
    }
</script>

<style scoped>
  #pre{
    position:absolute;
    top:10px;
    left: 20%;
  }
  #page{
    position: absolute;
    top: 1200px;
    left: 20%;
  }
</style>
