<template>
    <div class="article-card" @click="openModal">
    </div>
    <div class="article-modal" v-if="showModal" @click="closeModal">
      <div class="modal-overlay"></div>
      <div class="modal-content">
        <span class="close">&times;</span>
        <div class="article-header">
          <h2>{{ article.title }}</h2>
        </div>
        <div class="article-image">
          <img :src="article.image" alt="Article Image">
        </div>
        <div class="article-content">
          <p>{{ article.content }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ArticleModal',
    props: {
      article: {
        type: Object,
        required: true
      },
      showModal: {
        type: Boolean,
        required: true
      }
    },
    methods: {
      openModal() {
        this.$emit('open');
      },
      closeModal() {
        this.$emit('close');
      }
    }
  }
  </script>
  
  <style scoped>
 
  /* Gaya untuk modal */
  .article-modal {
  position: fixed;
  top: 0;
  left: 21.15%;
  width: 60%;
  height: 100%;
  display: flex;
  align-items: center; /* Tengah vertikal */
  justify-content: center; /* Tengah horizontal */

  }
  
  .modal-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
  }
  
  .modal-content {
    background-color: #FDF7E4;
    border-radius: 10px;
    padding: 20px;
    max-width: 80%;
    max-height: 80%;
    overflow-y: auto;
    box-shadow: 0 0 20px rgba(0, 0, 0,);
    position: relative;
    
  }
  
  .close {
    position: absolute;
    top: 10px;
    right: 10px;
    font-size: 20px;
    cursor: pointer;
    color: #333;
  }
  
  .article-header {
    text-align: center;
  }
  
  .article-header h2 {
    margin-bottom: 20px;
    color: black;
  }
  
  .article-image img {
   
    width: 50%;
    height: auto;
    border-radius: 5px;
    margin-bottom: 10px;
  }
  
  .article-content p {
    font-size: 16px;
    line-height: 1.6;
    color: #333;
    text-align: justify;
  }
  </style>
  