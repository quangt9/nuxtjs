<template>
<div>
    <popul-test v-show="show" @close-modal="changeShow" />
      <h3>ok e</h3>
    <div class="save-btn">
        <button @click="changeShow()">Save</button>
    </div>
      <h3>ok e</h3>
</div>
</template>

<script>
import PopulTest from '../components/PopulTest.vue'
export default {
  components: { PopulTest },
    data() {
        return {
            show: false
        }
    },
    methods: {
        changeShow() {
            this.show = !this.show
        }
    },
}
</script>
