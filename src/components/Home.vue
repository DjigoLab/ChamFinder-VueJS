<template lang="html">

  <section class="home">
    <section class="logo">
    <h1>ChamFind</h1>
</section>

<section class="menu-selection">
  <ul class="options">
    <li class="option"><i data-feather="search"></i>
    <p> Search </p>
    </li>
    <li class="option"><i data-feather="briefcase"></i>
        <p> Backpack </p>
</li>
    <li class="option"><i data-feather="users"></i>
        <p> Friends </p>
</li>
    <li class="option"><i data-feather="settings"></i>
        <p> Settings</p>
</li>
</ul>
  </section>
  </section>

</template>

<script lang="js">

  export default  {
    name: 'home',
    props: [],
    mounted() {

    },
    data() {
      return {
        value1: 0,
        value2: 1,

      }
    },
    methods: {

    },
    computed: {

    }
}
</script>

<style scoped >
.home {
  display: flex;
  flex-flow: column;
}
h1 {
  margin:15px 0px;
}
.logo {
  font-size: 8vh;
}
.menu-selection {
  justify-self: center;
}
.options {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  padding-left: 0px;
  grid-gap: 30px;
  list-style: none;
  padding: 30px;
}
.option {
  padding: 30px;
  background: #DCEDC8;
border-radius: 45px/15px;
}
</style>
