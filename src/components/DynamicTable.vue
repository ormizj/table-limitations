<template>
  <div class="dynamic-table">
    <table>
      <tr>
        <th>Header 1</th>
        <th>Header 2</th>
        <th>Header 3</th>
      </tr>
      <tr>
        <td>Data 1</td>
        <td>Data 2</td>
        <td>Data 3</td>
      </tr>
      <tr>
        <td class="long">Long Data</td>
      </tr>
      <tr>
        <td>Data 1</td>
        <td>Data 2</td>
        <td>Data 3</td>
      </tr>

    </table>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
table {
  padding: 15px;
  border: 1px solid white;
  background-color: gray;
}


tr {
  /* following styles don't work */
  padding: 999px;
  margin: 999px;
  border: 999px solid white;
}

td {
  /* margin doesn't work */
  margin: 5px;

  padding: 10px;
  border: 1px solid white;
}

th {
  padding: 10px;
}

.long {
  /* making a long data for dynamic table doesn't work (makes all colums longer [columns width will be equal to the widest data]) */
  width: 100px;
}
</style>
