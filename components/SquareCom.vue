<template>
    <div
      class="square1"
      :style="{background: activeColor}"
      @click="changeColor">
      
    </div>
</template>
<script>
export default {
  props: {
    firstColor: {
      type: String,
      required: true
    },
    secondColor: {
      type: String,
      required: true
    },
  },
  data(){
    return {
      isActive: true,
      activeColor: this.firstColor,
    }
  },
  methods: {
    changeColor() {
      if(this.activeColor===this.firstColor){
        this.activeColor=this.secondColor;
      } else {
        this.activeColor=this.firstColor;
      }
    }
  }

}
</script>
<style>
.square1 {
  margin      : auto;
  margin-bottom: 2em;
  width       : 200px;
  height      : 70px;
}
 
</style>
