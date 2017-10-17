<template>
  <div>
    <div class="title">
      <h1>This is Admin/Edit/{{$route.params.id}}</h1>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'edit',
    created () {
      console.log('Da li je konstruktor ?')
      console.log(this.$route.params)
    },
    data () {
      return {
        msg: 'Welcome to Admin page - online store from scotch.io'
      }
    }
  }
</script>