<template>
  <p>
    You are using electron v{{ versions['atom-shell'] }} with node v{{ versions.node }} on the {{ platform }} platform.<br>
    This is an early version of role play manager. If you want to help, contact me at charlesdelormefr@gmail.com
  </p>
</template>

<script>
  import os from 'os'

  export default {
    data () {
      return {
        platform: os.platform(),
        versions: process.versions
      }
    }
  }
</script>
