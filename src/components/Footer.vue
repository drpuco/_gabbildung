<template>
   
      <v-footer
        color="green"
        dark
      >
        <v-row
          justify="center"
          class="my-4 text-center"
        >
          <v-col cols="2">
            <v-btn
              href="#"
              v-for="link in links"
              :key="link"
              text
              dark
              >{{ link }}
            </v-btn>
          </v-col>
          <v-col cols="2">&copy; 2023 Gab Bildung</v-col>
        </v-row>
      </v-footer>

  </template>
  
  <script>
  export default {
    data: () => {
      return { links: ['Home', 'Blog', 'About'] };
    },
  };
  </script>