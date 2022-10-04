<template>
    <input @input="handleInput" />
</template>

<script>
export default {
  // prop: ['hidden'],
  // model: {
  //     prop: 'hidden',
  //     event: 'blur'
  // },
  // methods: {
  //     handleInput (value) {
  //         this.$emit('blur', value)
  //     }
  // }
  prop: ['value'],
  data () {
    return {
      content: this.value
    }
  },
  methods: {
    handleInput (e) {
      this.$emit('input', e.target.value)
    }
  }
}
</script>