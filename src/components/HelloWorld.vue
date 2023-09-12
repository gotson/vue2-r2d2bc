<template>
  <div id="D2Reader-Container">
    <main style="height: 100vh; tabindex: -1" id="iframe-wrapper"/>
  </div>
</template>

<script>
import D2Reader from '@d-i-t-a/reader'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  mounted () {
    D2Reader.load({
      url: new URL("http://localhost:15080/QSBDbGFzaCBvZiBLaW5ncyAtIEdlb3JnZSBSLiBSLiBNYXJ0aW4uZXB1Yg/manifest.json"),
    })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
