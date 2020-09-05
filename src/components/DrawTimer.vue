<template>
  <div>
    {{ timerCount }}
  </div>
</template>

<script>

  export default {
  name: 'DrawTimer',

  data() {
  return {
        timerCount: 600
      }
    },
    watch: {
      timerCount: {
        handler(value) {
          if (value > 0) {
            setTimeout(() => {
              this.timerCount--;
            }, 1000);
          }

        },
        immediate: true // This ensures the watcher is triggered upon creation
      }
    }
  }

</script>
