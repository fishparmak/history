<template>
	<div class="datas">
 		<h3> {{ data }} </h3>
 	</div>
</template>

<script>
export default {
  name: 'datas',
  data () {
    return {
      data: 'March 2016'
    }
  }
}
</script>

<style lang="scss">
.datas {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #979797;
  margin-top: 60px;
  background-image: url('/assests/Oval.png');
}

</style>
