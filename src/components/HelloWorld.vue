<template>
  <div>
    <b-table striped hover :items="items"></b-table>
  </div>
</template>

<script>
import data from "./json/data.json";

data.sort((a, b) => (a.Percentage < b.Percentage) ? 1 : (a.Percentage === b.Percentage) ? ((a.Duration > b.Duration) ? 1 : -1) : -1 ).map((e,index) => {e.Position = index+1;})
export default {
  name: "leaderboard",
  data() {
    return {
      items: data
    };
  },
};
</script>
<style >
thead tr {
  background-color: #00BCD4;
  color: white;
}
</style>
