<template>
  <binding></binding>
</template>

<script lang="ts">
import {Options, Vue} from 'vue-class-component';
import Binding from "@/components/Binding.vue";

@Options({
  components: {
    Binding,
  },
})
export default class App extends Vue {
}
</script>
