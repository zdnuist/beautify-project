<template>
  <div id="app">

    <b-navbar toggleable="md" type="dark" variant="info">
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand href="#">Beautiful</b-navbar-brand>

      <b-collapse is nav id="nav_collapse">

        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
        </b-navbar-nav>

      </b-collapse>

    </b-navbar>

    <div id="contain">

    <div id="manager">
      <BpNav></BpNav>
    </div>

      <div id="content">
        <router-view/>
      </div>
    </div>

  </div>
</template>

<script>
import BpNav from "./components/bp-nav";

export default {
  components: {BpNav},
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-left: 60px;
  margin-right: 60px;
}

#contain{
  margin: auto;
  overflow: hidden;
  width: 100%;
}


#manager {
  margin-top: 20px;
  width: 18%;
  float: left;

}

#content{
  margin-top: 20px;
  width: 82%;
  float: left;
  padding-left: 20px;
}
</style>
