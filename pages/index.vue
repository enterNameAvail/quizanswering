<template>
  <div class="component-space">
      <div class="gazo-box">
        <square-com first-color="red" second-color="green"/><br>
        <square-com first-color="blue" second-color="yellow"/><br>
        <square-com first-color="black" second-color="purple"/><br>
        <square-com first-color="gray" second-color="white"/><br>
        <square-com first-color="lightgreen" second-color="cyan"/><br>
      </div>

      <div class="gazo-box">
        <square-com first-color="orange" second-color="purple"/><br>
        <square-com first-color="lightblue" second-color="#CEF9DC"/><br>
        <square-com first-color="cyan" second-color="purple"/><br>
        <square-com first-color="fuchsia" second-color="red"/><br>
        <square-com first-color="purple" second-color="olive"/><br>
      </div>
    </div>
</template>

<script>
import SquareCom from '~/components/SquareCom'

export default {
  name: 'HomePage',
  components: {
    SquareCom,
  },
}
</script>

<style type="text/css">
  div.gazo-box {
    float: left;
    padding-right: 200px;
    justify-content: center;
  }

  div.component-space{
    padding: 300px 500px;
  }
</style>