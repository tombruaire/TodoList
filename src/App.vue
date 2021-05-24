<template>
  <div>
    <todos v-model="todos"></todos>
  </div>
</template>

<script>
import Todos from './components/Todos'

export default {
  data () {
    return {
      todos: [{
        name: 'Demo',
        completed: true
      }]
    }
  },
  methods: {
    addTodo () {
      this.todos.push({
        name: 'Tom',
        completed: false
      })
    }
  },
  components: {
    Todos
  }
}
</script>

