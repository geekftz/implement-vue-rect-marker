<template>
  <div id="app">
    <div class="wrap-box">
			<rectangle-marker v-model="mockData" :imgUrl="imgUrl"></rectangle-marker>
		</div>
  </div>
</template>

<script>
import RectangleMarker from '@/components/rectangleMarker'
export default {
  name: 'App',
  data() {
    return {
      imgUrl: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1598703959150&di=60209a30e75f4f10fc3c7ba9497a57b2&imgtype=0&src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201703%2F25%2F20170325211558_BzJVU.jpeg',
      mockData: [],
      // mockData: [["0.752500","0.566667"],["0.975000","0.566667"],["0.975000","0.995000"],["0.752500","0.995000"]]
    }
  },
  components: {
    RectangleMarker
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.wrap-box {
  height: 600px;
  width: 800px;
  background: gray;
}
</style>
