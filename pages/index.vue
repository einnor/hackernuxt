<template>
    <div class="f1 code">
        Hello World
        <li v-for="user in users" :key="user.id">
            {{ user.login }}
        </li>
    </div>
</template>

<script>
  import {mapState} from 'vuex'

  export default {
    computed: mapState([
      'users'
    ])
  }
</script>