<script>
export default {
    data() {
	    return{
        text : 'xxx',
      }
    },
  methods: {
    change1: function() {

      this.text = 'молодец, ты изменил текст';
    },
    change2: function() {
      this.text = 'ВАААУУ ТЫ МОГ ЕЩЁ АЗ ИЗМЕНИТЬ ТЕКСТ, ДА ТЫ ЛУЧШИЙ';
    } 
  } 
}
</script>

<template>
  <h1> {{text}} </h1>
  <br>
  <button @click="change1">text1</button>
  <button @click="change2">text2</button>
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
