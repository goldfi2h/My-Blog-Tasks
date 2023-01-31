<!-- <template>
    <div v-for="item in listItems" :key="item.id">
      {{item.title}}
    </div>
  </template>
  <script>
    export default {
      data() {
        return {
          listItems: []
        }
      },
      methods: {
        async getData() {
          const res = await fetch("http://my-fire.test/api/blog");
          const finalRes = await res.json();
          this.listItems = finalRes;
        }
      },
      mounted() {
        this.getData()
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
  </style>
   -->