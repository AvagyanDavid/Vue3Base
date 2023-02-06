<script>
export default {
    data() {
	    
    },
  methods: {
    show: function(int) {
      alert(int * int );
    }
  } 
}
</script>

<template>
  <h1> {{text}} </h1>
  <br>
  <button @click="show(2)">квадрат двойки</button>
  <button @click="show(3)">квадрат тройки</button>
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
