<script>
import Buttons from '~/components/Buttons.vue'
import PersonalBlock from '~/components/PersonalBlock.vue'
import SkillsBlock from '~/components/Skills.vue'

export default {
  components: {
    Buttons,
    PersonalBlock,
    SkillsBlock,
  },
}
</script>

<template lang="pug">
div
  .header
  .container
    Buttons
    PersonalBlock.top-margin
    span.block-title.top-margin SKILLS
    SkillsBlock.top-margin.bottom-margin
    //- .top-margin .
</template>

<style scoped>
.header {
  background: #011500;
  height: 400px;
  width: 100%;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.12), 0 0 6px rgba(0, 0, 0, 0.04);
}
.container {
  display: flex;
  flex-direction: column;
  width: 70%;
  height: 500px;
  margin: 0 auto;
  margin-top: -300px;
}
.top-margin {
  margin-top: 50px;
}
.bottom-margin {
  margin-bottom: 50px;
}
.block-title {
  text-align: center;
  font-size: 24px;
  font-weight: 100;
  color: #445588;
}
</style>
