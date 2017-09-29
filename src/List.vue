<template>
  <div>
      <div v-for="i in items">
          <div>{{i}}</div>
      </div>
      <button @click="run">run</button>
  </div>
</template>

<script>
export default {
    props : ["items"],
    mounted(){
        window.vm = this;
    },
    methods : {
        run(){
            console.log("Run")
            this.items.add(this.items.length);
        }
    }
}
</script>

<style>

</style>
