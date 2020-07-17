<template>
<html>
  <div class="hello">
    <b-table striped hover :items="items"></b-table>
  </div>
</html>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          Name: "Rohan",
          Score: 10,
          Duration: 30
        }
      ]
    };
  }
};
</script>


<style scoped>
th {
  background-color: teal;
}
</style>
