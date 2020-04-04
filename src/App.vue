<template>
  <div class="container">
    <app-notification :notification-type="notificationType" v-if="showNotification" @close-notification="showNotification=$event">
      Primar lorem ipsum dolor sit
    </app-notification>
  </div>
</template>

<script>
  import Notification from './components/Notification.vue'
  export default {
    data(){
      return {
        showNotification: true,
        notificationType: 'is-danger'
      }
    },
    components:{
      appNotification: Notification
    }
  }

</script>

<style>
</style>
