<template>
  <b-table striped hover :items="items" :fields="fields"></b-table>

</template>
<script>
  export default  {
    name: 'users',
    data () {
      return {
        fields: [
          {key: 'name' , label: ' 用户名' },
          {key: 'sex', label: '性别'} ,
          {key: 'age', label: '年龄'}],
        items: [
          {name: 'zd', sex: 'man', age: 18},
          {name: 'zs', sex: 'woman', age: 34}
        ]
      }
    }
  }
</script>
