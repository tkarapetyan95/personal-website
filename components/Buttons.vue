<template lang="pug">
.name-and-buttons
  .name
    span.fname Tigran
    span.lname  Karapetyan
    p.prof software developer
  .buttons
    el-tooltip(content='kar.tigran' placement='top')
      .social-btn
        a(href='https://facebook.com/kar.tigran' target='blank')
          img(src='https://img.icons8.com/ios/100/000000/facebook-f.png')
    el-tooltip(content='@tkarapetyan95' placement='top')
      .social-btn
        a(href='https://instagram.com/tkarapetyan95/' target='blank')
          img(src='https://img.icons8.com/ios/100/000000/instagram-new.png')
    el-tooltip(content='/tigran.karapetyan' placement='top')
      .social-btn
        a(href='https://vk.com/tigran.karapetyan' target='blank')
          img(src='https://img.icons8.com/ios/100/000000/vk-com.png')
</template>

<style scoped>
.name-and-buttons {
  display: flex;
  align-items: center;
  height: 65px;
}
.lname {
  font-weight: 400;
}
.name {
  font-size: 36px;
  color: whitesmoke;
  font-family: 'Roboto';
  font-weight: 100;
}
.prof {
  font-size: 16px;
  margin-left: 3px;
  font-family: 'Courier New', Courier, monospace;
}
.buttons {
  margin-left: auto;
  display: flex;
  align-items: baseline;
}
img {
  width: 28px;
  margin: 5px 5px;
  filter: invert(1);
}
.social-btn {
  width: 40px;
  height: 40px;
}
.social-btn:hover {
  background: rgba(255, 255, 255, 0.05);
}
</style>
