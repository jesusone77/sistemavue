<template>
  <about-bar></about-bar>
</template>
<script>
  import AboutBar from '../components/About-Bar'

  export default {
    name: 'Home',

    components: {
      AboutBar,
    },
    data () {
      return {
        
      }
    },
    methods: {
      getTitle() {
        return this.title;
      }
    },
    computed: {
      customTitle() {
        return title = 'Index CRUD';
      }
    }
  }
</script>
