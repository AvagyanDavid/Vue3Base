<script>
  export default{
    data(){
      return{
        mas: [1, 2, 3],
        arr: ['x', 'y', 'z'],
      }
    }
  }
</script>

<template>
  <div>
    <p>{{arr[0]}}</p>
    <p>{{arr[1]}}</p>
    <p>{{arr[2]}}</p>
  </div>
    {{mas[0]+ mas[1]+mas[2]}}
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
