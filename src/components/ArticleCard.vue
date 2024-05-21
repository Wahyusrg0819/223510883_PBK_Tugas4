<template>
    <div class="article-card">
      <div class="article-image">
        <img :src="article.image" alt="Article Image">
      </div>
      <div class="article-content">
        <h2>{{ article.title }}</h2>
        <p class="summary">{{ article.summary }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ArticleCard',
    props: {
      article: {
        type: Object,
        required: true
      }
    }
  }
  </script>
  
  <style scoped>
  .article-card {
    width: 300px;
    height: 400px;
    background-image: linear-gradient(163deg, #00ff75 0%, #3700ff 100%);
    border-radius: 20px;
    overflow:hidden; /* Menghindari konten yang melebihi batas kartu */
    transition: all 0.3s;
    margin-bottom: 40px;
    margin-right: 0%;
    margin-left: 0%;
    cursor: pointer;
  }
  
  .article-card:hover {
    box-shadow: 0px 0px 30px 1px rgba(0, 255, 117, 0.99);
  }
  
  .article-image img {
    width: 100%;
    height: auto;
    border-radius: 20px 20px 0 0;
  }
  
  .article-content {
    padding: 20px;
    padding-top: 10px;
    padding-bottom: 10px;
  } 
  
  .article-content h2 {
    font-size: 16px;
    margin-bottom: 10px;
    color: #fff;
    overflow: hidden; /* Menghindari teks judul yang melebihi batas kartu */
    text-overflow: ellipsis; /* Menambahkan elipsis untuk teks judul yang terpotong */
    text-align:center; 
  }
  
  .article-content .summary {
    font-size: 14px;
    color: #fff;
    overflow: hidden; /* Menghindari teks ringkasan yang melebihi batas kartu */
    text-overflow: ellipsis; /* Menambahkan elipsis untuk teks ringkasan yang terpotong */
    text-align: justify;
    margin-bottom: 10px;
  }
  </style>
  