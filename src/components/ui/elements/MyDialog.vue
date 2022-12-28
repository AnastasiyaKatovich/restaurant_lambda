<template>
    <div class="dialog" v-if="show" @click="hideDialog">
        <div @click.stop class="dialog_content">
            <a href="#" @click="hideDialog" class="close">&times;</a>
            <slot>default</slot>
        </div>
    </div>
</template>

<script>
export default {
  name: "MyDialog",
  props: {
    show: {
      type: Boolean,
      default: false
    }
  },
  methods:{
    hideDialog(){
      this.$emit('update:show', false);
    }
  }
}
</script>

<style>
.close{
  float: right;
  text-decoration: none;
  color: red;

}
/* .close::after{
  content: "close";
} */
.dialog {
  top: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.5);
  position: fixed;
  display: flex;
  height: 100%;
}
.dialog_content {
  margin: auto;
  background: white;
  border-radius: 12px;
  min-height: 50px;
  min-width: 500px;
  padding: 20px;
  z-index: 100;
}
</style>