<template>
  <div>
    <h1>{{ message }}</h1>
    <app-input :msg="message" @messageChanged="message = $event"></app-input>
  </div>
</template>

<script>
  import Input from './Input';

  export default {
    data() {
      return {
        message: 'Das is ne krasse nachricht.. '
      }
    },
    components: {
      'app-input': Input
    }
  }
</script>
