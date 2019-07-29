<template>
  <div>
    <Header id="header">

    </Header>
    <Preview id="pre">
    </Preview>
    <Page id="page">
    </Page>

      <DatePicker id="date">

      </DatePicker>
  </div>
</template>

<script>
  import Preview from './Preview.vue';
  import Page from './Page.vue';
  import Header from './Header.vue';
  import DatePicker from './DatePicker.vue'
  export default {
      components: {Preview,Page,Header,DatePicker},
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
    top: 1300px;
    left: 30%;
  }
  #header{
    position: fixed;
    top:0px;
    width: 100%;
    left: 0%;
    z-index:9999
  }
  #date{
    position:absolute;
    top:70px;
    width: 20%;
    height: 50%;
    left: 75%;
  }
</style>
