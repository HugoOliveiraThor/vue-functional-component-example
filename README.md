# Simple example of VueJS functional components 

- Example - A file called FunctionalComponent.vue
```
<template functional>
  <div>
    <p v-for="brand in props.brands" :key="brand">{{brand}} </p>
  </div>
</template>
<script> 
export default {
  functional: true,
  name: 'Test',
  props: {
    brands: Object
  }  
}
</script>
```
- We can import in our App.vue 
```
<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <functional-component 
     :brands ="['Tesla', 'Bentley', 'Ferrari', 'Ford']">
    </functional-component>
  </div>
</template>

<script>
import FunctionalComponent from './components/FunctionalComponent.vue'

export default {
  name: 'App',
  components: {
    FunctionalComponent
  }
}
</script>
```




### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
