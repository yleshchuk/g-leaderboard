<template>
  <v-container class="fill-height">
    <v-responsive class="align-center text-center fill-height">
      <v-table theme="dark">
        <thead>
          <tr>
            <th class="text-left">Name</th>
            <th class="text-left">Best</th>
            <th class="text-left">Total</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="item in players" :key="item.name">
            <td>{{ item.name }}</td>
            <td>{{ item.total }}</td>
            <td>{{ item.best }}</td>
          </tr>
        </tbody>
      </v-table>
    </v-responsive>
  </v-container>
</template>

<script lang="ts" setup>
const players = [{ name: "Yarko", best: 15555, total: 35000 }];
</script>
