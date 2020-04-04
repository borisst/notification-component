<template>
  <div class="notification" :class="notificationClass">
    <button class="delete" @click="closeNotification"></button>
    <slot>Primar lorem ipsum dolor sit amet, consectetur</slot>
  </div>
</template>
<script>
  export default {
    props:{
      notificationType:String,
    },
    data(){
      return{
        notificationClass: this.notificationType
      }
    },
    methods:{
      closeNotification(){
        this.$emit('close-notification',false)
      }
    }
  }
</script>
