<template>
    <nav>
        <v-menu>
      <template v-slot:activator="{ props }">
        <v-btn
          color="primary"
          v-bind="props"
        >
          Activator slot
        </v-btn>
      </template>
      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
          :value="index"
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
    </nav>
</template>
<script>
 export default {
    data: () => ({
      items: [
        { title: 'Click Me' },
        { title: 'Click You' },
        { title: 'Click Me' },
        { title: 'Click U 2' },
      ],
    }),
  }
</script>