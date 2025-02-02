<template>
  <section id="todoDav">
    <h2 class="text-xl font-bold">To-Do List</h2>
    <ul class="space-y-2 mt-4">
      <li
        v-for="(task, index) in tasks"
        :key="index"
        class="flex justify-between items-center bg-gray-100 p-2 rounded"
      >
        <input
          type="checkbox"
          v-model="task.completed"
          class="mr-2"
        />
        <span :class="{ 'line-through': task.completed }">{{ task.name }}</span>
        <button
          @click="removeTask(index)"
          class="bg-red-500 text-white px-2 py-1 rounded"
        >
          Remove
        </button>
      </li>
    </ul>
    <div class="mt-4">
      <input
        v-model="newTask"
        type="text"
        placeholder="Add a new task"
        class="border p-2 w-full"
      />
      <button
        @click="addTask"
        class="mt-2 bg-blue-500 text-white px-4 py-2 rounded"
      >
        Add Task
      </button>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Todo',
  data() {
    return {
      newTask: '',
      tasks: [],
    };
  },
  methods: {
    addTask() {
      if (this.newTask.trim() !== '') {
        this.tasks.push({ name: this.newTask, completed: false });
        this.newTask = '';
      }
    },
    removeTask(index) {
      this.tasks.splice(index, 1);
    },
  },
};
</script>

<style scoped>
.line-through {
  text-decoration: line-through;
}
</style>
