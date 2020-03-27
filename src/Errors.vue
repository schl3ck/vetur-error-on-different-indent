<template>
  <div>
    <table>
      <tbody>
        <tr
          v-for="task in tasks"
          :key="task.id"
          @select="shouldError(task)"
          @other="errorsToo(42)"
          @something="noError">
          <td>some content</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>

export default {
  name: "TaskList",
  data: function() {
    return {
      tasks: []
    };
  },
  methods: {
    shouldError(task) {},
    errorsToo(id) {},
    noError() {}
  }
};
</script>
