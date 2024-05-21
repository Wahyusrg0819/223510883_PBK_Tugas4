<template>
  <div class="article-card-list">
    
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'ArticleCardList'
}
</script>

<style scoped>
.article-card-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin-top: 20px;
}
</style>
