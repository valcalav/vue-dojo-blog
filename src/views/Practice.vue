<template>
  <div>
    <h1>Home</h1>

    <!-- REF AND REACTIVE
    <h2>Refs</h2>

    <p> {{ ninjaOne.name }} - {{ ninjaOne.age }} </p>
    <button @click="updateNinjaOne">Update ninja one</button>

    <h2>Reactive</h2>
    <p> {{ ninjaTwo.name }} - {{ ninjaTwo.age }} </p>
    <button @click="updateNinjaTwo">Update ninja two</button> -->

    <!-- <h2>Computed values</h2>
    <input type="text" v-model="search">
    <div v-for="name in names" :key="name">
      {{name}}
    </div>
    <h3>Matching names</h3>
    <div v-for="name in matchingNames" :key="name">
      {{name}}
    </div> -->

  </div>
  
</template>

<script>
import { computed, ref, reactive } from '@vue/reactivity'
import { watch, watchEffect } from '@vue/runtime-core'


export default {
  name: 'Home',
  setup() {



    // REF AND REACTIVE

    // const ninjaOne = ref({name: 'mario', age: 30})
    // const ninjaTwo = reactive({ name: 'luigi', age: 35})
    
    // const updateNinjaOne = () => {
    //   ninjaOne.value.age = 40
    // }

    // const updateNinjaTwo = () => {
    //   ninjaTwo.age = 45
    // }

    // return { ninjaOne, updateNinjaOne, ninjaTwo, updateNinjaTwo }

    // WATCH AND WATCHEFFECT 
    
    // const search = ref('')
    // const names = ref(['mario', 'luigi', 'yoshi', 'toad', 'peach', 'bowser'])

    // watch(search, () => {
    //   console.log('watch function ran')
    // })

    // watchEffect(() => {
    //   console.log('watchEffect function ran', search.value)
    // })

    // const matchingNames = computed(() => {
    //   return names.value.filter(name => name.includes(search.value))
    // })

    // return { names, search, matchingNames }
  
  }
}
</script>
