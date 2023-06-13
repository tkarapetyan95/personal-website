<script>
export default {
  data() {
    return {
      frontTags: [
        'JavaScript',
        'Vue',
        'WebPack',
        'service worker',
        'PWA',
      ],
      backTags: [
        'C#',
        '.NET Core',
        'ASP.NET',
        'Entity Framework',
        'Dapper',
        'Postgres SQL',
        'MSSQL',
        'Mongo DB',
        'Mongo C# Driver',
      ],
      otherTags: [
        'Docker',
        'Kafka',
        'REST',
        'ELK',
        'IIS',
        'Git',
        'TFS',
        'Scrum',
        'Azure',
        'Firebase',
      ],
    }
  },
}
</script>

<template lang="pug">
.block
  el-row
    el-col(span='8')
      .title
        span Front-end
      .tags: el-tag(v-for='tag in frontTags' type='info' effect='dark') {{ tag }}
    el-col(span='8').middle-block
      .title
        span Back-end
      .tags: el-tag(v-for='tag in backTags' type='info' effect='dark') {{ tag }}
    el-col(span='8')
      .title
        span Others
      .tags: el-tag(v-for='tag in otherTags' type='info' effect='dark') {{ tag }}
</template>

<style scoped>
.block {
  height: 350px;
  flex-direction: column;
  background: whitesmoke;
  box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
}

.title {
  background: rgba(0, 0, 0, 0.1);
  text-align: center;
  padding: 10px;
}

.el-tag {
  margin: 5px 7px;
  border-radius: 50px;
}

.el-row {
  background: white;
  margin: 1px;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  padding: 0 10px;
}

.middle-block {
  background: whitesmoke;
}
</style>
