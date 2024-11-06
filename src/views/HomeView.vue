<template>
  <div class="home">
    <MdEditor :value="value" :handle-change="onChange" />
    <CodeEditor />
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import MdEditor from "@/views/user/MdEditor.vue";
import CodeEditor from "@/views/user/CodeEditor.vue"; // @ is an alias to /src

const value = ref();
const onChange = (v: string) => {
  value.value = v;
};
</script>
