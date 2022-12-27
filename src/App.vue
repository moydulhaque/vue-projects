<template>
  <div>
    <h2 class="font-bold text-red-500">{{ msg }}</h2>
  </div>
</template>

<script>
export default {
  name:'App',
  data(){
    return {
      msg: 'Welcome to Vue.js'
    }
  },
  methods: {
    test() {
      console.log('test')
    }
  }
}
</script>