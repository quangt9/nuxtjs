<template>
<div class="modal-overlay">
    <div class="close-button" @click="closePopul">sưdeasd</div>
    <div class="popul-modal">
        <div class="close-button" @click="closePopul">sưdeasd</div>
        <div class="modal-content">
                aliceblu
                <h5 @click="closePopul">xzy</h5>
            </div>     
    </div>
</div>
</template>

<script>
export default {
    methods: {
        closePopul() {
            this.$emit('close-modal')
        }
    },
}
</script>

<style scoped>
</style>
