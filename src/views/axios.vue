<template></template>
<script lang="ts">
import { defineComponent } from 'vue';
import axios from '../utils/axios';

export default defineComponent({
  setup() {
    axios
      .get('/users/XPoet')
      .then((res) => {
        const i = 2;
        console.log('res: ', res);
      })
      .catch((err) => {
        console.log('err: ', err);
      });
  },
});
</script>
