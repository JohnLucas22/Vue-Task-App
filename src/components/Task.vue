<template>
  <div class="task">
    <h3>{{ task.text }} <i class="fas fa-times"></i></h3>
    <p>{{ task.day }}</p>
  </div>
</template>

<script>
export default {
  name: "Task",
  props: {
    task: Object,
  },
};
</script>

<style scope>
.fas {
  color: red;
}
.task {
  background: #f4f4f4;
  margin: 5px;
  padding: 10px 20px;
  cursor: pointer;
}
.task.reminder {
  border-left: 5px solid green;
}
.task h3 {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>

<!-- Video Link: https://www.youtube.com/watch?v=qZXt1Aom3Cs -->
<!-- Minute Mark: 44:44 -->
