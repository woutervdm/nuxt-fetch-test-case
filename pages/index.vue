<template>
  <div class="container">
    <button
      type="button"
      @click="click"
    >
      Add component
    </button>
    <hello-world
      v-for="i of number"
      :key="i"
    />
  </div>
</template>

<script>
export default {
  data: () => ({
    number: 1
  }),
  methods: {
    click () {
      this.number++
    }
  }
}
</script>
