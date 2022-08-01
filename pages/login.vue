<template>
<div>
    <div class="container" @mousemove="someMethod">
        <div class="main">
            <div class="bottom" ref="control">
                <div class="control"  v-on:mousedown="hold = true"  @touchcancel="hold = false"
  v-on:mouseup="hold = false">11111</div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            hold: false,
        }
    },
    methods: {
        someMethod(event) {
            let maxHeight = window.innerHeight;
           
            if (this.hold) {
                console.log(event.clientY);
                this.$refs.control.style.height = (maxHeight - event.clientY) + 'px';
                console.log('height:' + this.$refs.control.clientHeight);
            }

        }
    }
}
</script>

<style>
html,
body,
.container {
    height: 100%;
    width: 100%;
    /* background-color: red; */

}
    .main {
        height: 100vh;
        background-color: bisque;
    }

.bottom {
    width: 200px;
    height: 300px;
    background-color: antiquewhite;
    bottom: 0;
    position: absolute;
}
</style>
