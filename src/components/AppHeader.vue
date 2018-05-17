<template lang="html">

  <section class="app-header">
    <router-link to="/">Home</router-link>
    <span>Logo</span>
    <router-link to="/login">User</router-link>
  </section>

</template>

<script lang="js">
  export default  {
    name: 'app-header',
    props: [],
    mounted() {

    },
    data() {
      return {

      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped >
  .app-header {

    display: flex;
    justify-content: space-between;
    background: #795548;
    color: #DCEDC8;
   padding: 15px;}
   a{
     color: #DCEDC8;
   }

</style>
