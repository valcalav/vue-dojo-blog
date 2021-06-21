<template>
  <div class="home">
    <h1>home</h1>
    <p ref="p">{{name}} and {{age}}</p>
    <button @click="handleClick">click me</button>
    <button @click="age++">Increase age</button>
    <input type="text" v-model="name">
  </div>
  
</template>

<script>
import { ref } from '@vue/reactivity'


export default {
  name: 'Home',
  setup() {

    // console.log(this)

    // const p = ref(null)

    let name = ref('mario')
    let age = ref(30)

    const handleClick = () => {
      name.value = 'luigi'
      age.value = 33
      // console.log(p, p.value)
      // p.value.classList.add('test')
      // p.value.textContent = 'hello, ninjas'
    }

    return { name, age, handleClick }
  }
}
</script>
