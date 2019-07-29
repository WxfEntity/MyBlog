<template>
  <el-calendar v-model="value" class="datePick">
  </el-calendar>
</template>

<script>
    export default {
      data() {
        return {
          value: new Date()
        }
      }
    }
</script>

<style scoped>
</style>
