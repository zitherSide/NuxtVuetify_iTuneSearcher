<template>
  <v-app dark>
    <div>
      <ToolBar/>
      <nuxt/>
    </div>
  </v-app>
</template>

<script>
import ToolBar from '~/components/ToolBar.vue';

export default {
  data () {
    return {  }
  },
  components:{
    ToolBar
  }
}
</script>
