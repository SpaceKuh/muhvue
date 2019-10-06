<template>
  <div id="muh">
    <a @click="handleClick()">Click me! {{name}}</a>
    <button @click="pressButton()"> {{title}}</button>
  </div>
</template>

<script>
// export default {
//   name: 'HelloWorld',
//   props: {
//     msg: String
//   }
// }

export default {
  props:{
    title: String
  },
  data() {
    return {
      name: 'Muh'
    }
  },
  methods: {
    handleClick: function() {
      console.log(this.name)
    },
    pressButton: function()
    {
     this.name = "Katze";
    }
  }
}

console.log("code is being called");
    let image = new Image();
        image.onload = (event) => {
            console.log("image loaded");
        }
        image.src = "static/prison_tileset.png";
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
