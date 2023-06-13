<script>
import RowItem from './utils/row'

export default {
  components: {
    RowItem,
  },
  data() {
    return {
      age: new Date().getFullYear() - new Date(1995, 12, 23).getFullYear(),
    }
  },
}
</script>

<template lang="pug">
.block
  .img
    img(src='~/static/profile_pic.jpg')
  .info
    p.first-line I'M 
      span TIGRAN KARAPETYAN
    p.prof Software Developer
    .line
    RowItem(title='Age' :value='`${age} (23 December)`')
    RowItem(title='Address' value='Yerevan, Armenia')
    RowItem(title='Email' value='kartigo.1995@gmail.com')
    RowItem(title='Phone1' value='+374 (91) 845-845')
    RowItem(title='Phone2' value='+7 (977) 877-68-60')
</template>

<style scoped>
.block {
  height: 350px;
  display: flex;
  background: white;
  box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
}

.img {
  width: 350px;
  border: 1px solid;
  border-color: lightgrey;
}

img {
  height: 100%;
}

.info {
  width: 100%;
  padding: 20px;
  font-size: 34px;
  font-family: 'Roboto';
}

p span {
  font-weight: bold;
  color: #445588;
}

.prof {
  font-size: 20px;
  font-weight: 100;
}

.line {
  width: 100%;
  border-top: 1px grey solid;
  margin: 15px 0;
}
</style>
