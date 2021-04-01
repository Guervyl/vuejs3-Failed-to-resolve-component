<template>
  <p>Api Binding</p>
  <p>Add Binding
    <button @click="parameters.push(1)"><span style="font-size: 2em; padding: 5px;">+</span></button>
  </p>

  <!-- This one here is the problem -->
  <binding v-for="(count,i) in parameters" :key="i"></binding>
</template>

<script lang="ts">
import {Options, Vue} from "vue-class-component";
import Binding from "@/components/Binding.vue";

@Options({
  props: ['modelValue'],
  components: {
    Binding
  }
})
export default class ApiBinding extends Vue {
  // This is just for demonstration. My parameters are not just an array of int.
  parameters: number[] = []
}
</script>