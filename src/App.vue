<template>
  <div id="app">
    <button type="button" class="btn" @click="showModal">打开Modal</button>
    <modal v-show="isModalVisible" @close="closeModal"></modal>
  </div>
</template>

<script>
import Modal from '@/components/Modal'

export default {
  name: 'App',
  components: {
    Modal
  },
  data () {
    return {
      isModalVisible: false
    }
  },
  methods: {
    showModal: function () {
      this.isModalVisible = true
    },
    closeModal: function () {
      this.isModalVisible = false
    }
  }
}
</script>

<style>

</style>
