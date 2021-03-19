<template>
  <div>
    {{ data }}
    <pre>{{ $fetchState }}</pre>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
    data: ''
  }),
  fetch () {
    this.data = 'Hello world!'
  }
}
</script>
