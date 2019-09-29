<script>
export default {
  props: ['title', 'value'],
}
</script>

<template lang="pug">
.row
  .title
    span {{ title }}
  .value
    span {{ value }}
</template>

<style scoped>
.title {
  /* color: darkgray; */
  width: 150px;
}
.row {
  display: flex;
  font-size: 20px;
  margin-bottom: 10px;
  font-family: Roboto;
  font-weight: 200;
}
</style>
