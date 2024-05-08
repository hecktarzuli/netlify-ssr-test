<template>
  <div>
    From Server: {{ test }}<br/>
    Refresh this page a couple of times, even view-source and refresh that.  You can see the test value keeps changing.
  </div>
</template>
<script setup>
const test = ref(0)
test.value = useState('test', () => Date.now())

</script>
