<template>
    <div class="pagination">
      <!-- <ul v-if="currentPage"> -->
      display:{{display}}
      <!-- </ul> -->
    </div>
</template>

<script>
  export default{
    data(){
      return {
      }
    },
    props: {
      display: {// 每页显示条数
        type: Number
      }
    },
    computed: {
    },
    methods: {
      inationAdd(index) {
        this.$emit('pagechange', index);
      }
    },
    mounted() {
    },
  }
</script>
<style>

</style>
