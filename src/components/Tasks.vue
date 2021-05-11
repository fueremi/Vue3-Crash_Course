<template>
  <div v-for="task in tasks" :key="task.id">
    <h3>
      <Task :task="task" />
    </h3>
  </div>
</template>

<script>
import Task from '@/components/Task'

export default {
  name: "Tasks",
  props: {
    tasks: Array,
  },
  components: {
    Task
  }
};
</script>