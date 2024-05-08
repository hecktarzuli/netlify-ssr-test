<template>
  <div>
    From Server: {{ test }}
  </div>
</template>
<script setup>
const test = ref(0)
test.value = useState('test', () => Date.now())

</script>
