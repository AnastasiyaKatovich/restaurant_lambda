<template>
    <select @change="changeOptions" v-model="SelectedValue">
        <options disabled value="">Выберите из списка</options>
        <options v-for="option in options" :key="option.id">{{option.name}}</options>
    </select>

</template>
<script>
export default {
  name: "FormSelect",
  data(){
    return {
      SelectedValue:''
    }
  },
  props: {
    options: {
      type: Array,
      default: () => []
    }
  },
  methods: {
    changeOptions() {
      this.$emit('update:modelValue', this.SelectedValue);
    }
  }
}
</script>