<template>
  <div class="container mx-auto">
  <div class="mt-10">
    <h2 class="font-bold text-red-500">{{ msg }}</h2>
  </div>
  <div class="mt-10">
    <button class="border p-2" @click="test">Click Me</button>
  </div>
  <div class="mt-10">
    <h2 class="mb-4 text-2xl ">List of Courses</h2>
    <ul>
      <li v-for="course in courses" class="shadow p-4 mb-4 border border-gray-200">
        {{ course.name }} - {{ course.instructor }}
      </li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  name:'App',
  data(){
    return {
      msg: 'Welcome to Vue.js',
courses: [
      { name: 'Vue.js', instructor: 'Polash Mahmud' },
      { name: 'Laravel', instructor: 'Rasel Ahmed' },
      { name: 'HTML', instructor: 'John Doe' },
    ]
    }
  },
  methods: {
    test() {
      this.msg = 'Welcome Message Changed'
    }
  }
}
</script>