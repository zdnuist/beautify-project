<template>
  <div>
      <b-btn v-b-toggle.collapse1 variant="info">权限管理</b-btn>
      <b-collapse id="collapse1" class="mt-2">
        <b-list-group>
          <b-list-group-item>
            <router-link to="/users">用户管理</router-link></b-list-group-item>
          <b-list-group-item href="#">管理员管理</b-list-group-item>
        </b-list-group>

      </b-collapse>

  </div>

</template>


