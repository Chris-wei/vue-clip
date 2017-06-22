<template>
  <div class="hello">
      <img src="" alt="" id="img1">
      <input type="file" accept="image/png,image/jpg,image/jpeg" @change="change($event)" data-type="1">
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods : {
    change( event ) {
        let image = document.getElementById('img1');
        this.clip(event , {
          resultObj : image,
          aspectRatio : 1
        })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    img{
        display: block;
        width: 120px;
        height: 120px;
    }
    h3{
        text-align: center;
    }
    h1, h2 {
      font-weight: normal;
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
