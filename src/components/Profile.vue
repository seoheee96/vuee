<template>
  <div class="container">
    <header class="jumbotron">
      <h3>id : {{content.id}}</h3>
      <h3>name : {{content.name}}</h3>
    </header>
  </div>
</template>

<script>
import UserService from '../services/user-service.js'

export default {
  name: 'profile',
  data() {
    return {
      content: ''
    }
  },
  mounted() {
    UserService.getUserContent().then(
      response => {
        this.content = response.data
      },
      error => {
        this.content = error.response.data.message
      }
    )
  }
}
</script>