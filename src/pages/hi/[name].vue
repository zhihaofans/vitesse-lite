<script setup lang="ts">
const props = defineProps<{ name: string }>();
const router = useRouter();
import { NButton } from 'naive-ui';
</script>

<template>
  <div>
    <div i-carbon-pedestrian text-4xl inline-block />
    <p>
      Hi, {{ props.name }}
    </p>
    <p text-sm op50>
      <em>Dynamic route!</em>
    </p>

    <div>
      <n-button @click="router.back()">返回</n-button>
    </div>
  </div>
</template>
