<script>
export default {
    data() {
	    return {
		    cost: '500',
		    amount: '4',
	    }
    },
  computed: {
	  price: function() {
		  return this.cost * this.amount;
	  }
  }
}
</script>

<template>
  <p>Цена данного продукта {{ cost }}</p>
  <br>
	<p>Количество {{ amount }}</p>
  <br>
	<p>Стоимость {{ price }}</p>
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
