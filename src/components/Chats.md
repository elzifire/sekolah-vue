<template>
    <div class="whatsapp-icon" v-if="showIcon" @click="openWhatsapp">
        <i class="fa fa-whatsapp"></i>
      </div>
  </template>
  
  <script>
  export default {
    
    name: 'ChatsComponent',
    methods: {
      openwa() {
        // aksi yang dijalankan ketika icon di-klik
        const whatsappUrl = `https://wa.me/${this.phoneNumber}`
      window.open(whatsappUrl, '_blank')
      }
    },
    data() {
        return {
            phoneNumber: '6281234567890'
        }
    }
  }
  </script>
  
  <style>
  .floating-icon {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 50px;
    height: 50px;
    background-color: #25D366;
    color: #fff;
    border-radius: 50%;
    text-align: center;
    cursor: pointer;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.4);
    z-index: 9999;
  }
  
  .floating-icon i {
    font-size: 24px;
    line-height: 50px;
  }
  </style>
  