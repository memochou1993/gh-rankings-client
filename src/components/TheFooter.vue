<template>
  <v-footer
    color="primary primary-gradient"
    dark
    padless
  >
    <v-col
      class="font-weight-light text-center py-2"
    >
      <span
        class="pointer"
        @click="explore()"
        v-text="`© ${new Date().getFullYear()} GH Rankings`"
      />
    </v-col>
  </v-footer>
</template>

<script>
import {
  open,
} from '@/helpers';

export default {
  name: 'TheFooter',
  methods: {
    explore() {
      open('https://github.com/memochou1993/gh-rankings');
    },
  },
};
</script>
