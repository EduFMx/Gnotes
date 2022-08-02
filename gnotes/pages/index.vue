<template>
<div>

  <b-navbar toggleable type="dark" variant="dark">
    <b-navbar-brand href="#">Gnotes</b-navbar-brand>

    <b-navbar-toggle target="navbar-toggle-collapse">
      <template #default="{ expanded }">
        <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
        <b-icon v-else icon="chevron-bar-down"></b-icon>
      </template>
    </b-navbar-toggle>


    <b-collapse id="navbar-toggle-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Nintendo</b-nav-item>
        <b-nav-item href="#">PlayStation</b-nav-item>
        <b-nav-item href="#">Xbox</b-nav-item>
        <b-nav-item href="#">Pc</b-nav-item>

        <br>
        <br>

        <b-nav-item href="#">Configurações</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <br>
  <b-img v-bind="mainProps" blank-color="white" alt="Named color image (white)"></b-img>

</div>
 
   
</template>

<script>
export default {
  name: 'IndexPage',
  data(){
    return {
        mainProps: { blank: true, width: 90, height: 90, class: 'm1' }
    }
  }
}
</script>

<style scoped>

</style>
