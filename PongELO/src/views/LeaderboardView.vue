<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
<script>
  export default {
    mounted() {
      this.fetchData()
    },
    data() {
      return {
        allData:"",
        brotherOrdering:{},
      }
    },
    methods: {
      async fetchData() {
        try {
          const obj = await fetch(
            'https://raw.githubusercontent.com/BoundlessFate/PongELOData/main/data.json'
            ).then(res => res.json());
          console.log(obj.brother);
          this.data = obj;
          sortData();
        } catch (ex) {
          console.log("Error in fetch");
        }
      },
      sortData() {
        
      }
    }
  }
</script>