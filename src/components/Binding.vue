<template>
  <p>Binding</p>
  <ApiBinding></ApiBinding>
</template>

<script lang="ts">
import {Options, Vue} from "vue-class-component";
import ApiBinding from "@/components/ApiBinding.vue";

@Options({
  components: {
    ApiBinding
  }
})
export default class Binding extends Vue {
}
</script>