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
.modal-overlay {
    position: fixed;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: center;
    background-color: #fafafa00;
}

.popul-modal {
    width: 45vh;
    height: 70vh;
    /* background-color: aliceblue; */
    position: absolute;
    bottom: 0;
    margin-left: 50px;
    /* border-top-left-radius: 15px; */
}

.modal-content {
    width: 100%;
    height: 100%;
    background-color: white;
    border-top-left-radius: 5px;
}

.close-button {
    top: 5px;
    color: red;
}
</style>
