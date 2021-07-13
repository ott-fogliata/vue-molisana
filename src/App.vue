<template>
  <div id="app">
    <Header :navList="nav"/>
    <Main :products="products"/>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App', 
  components: {
    Header,
    Main,
    Footer
  },
  data: function() {
    return {
      nav: [
        {
            id: 0,
            name: 'Home',
            link: '/home'
        },
        {
            id: 1,
            name: 'Prodotti',
            link: '/product'  
        },
        {
            id: 2,
            name: 'Chi Siamo',
            link: '/who-we-are' 
        },
        {
            id: 3,
            name: 'Contatti',
            link: '/contacts' 
        }
      ],
      products: [
          {
              "id": 0,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.4 Spaghetto Quadrato Bucato",
              "tipo": "lunga",
              "cottura": 6
          },
          {
              "id": 1,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.5 Fettuccine",
              "tipo": "lunga",
              "cottura": 13
          },
          {
              "id": 2,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.6 Linguine",
              "tipo": "lunga",
              "cottura": 12
          },
          {
              "id": 3,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.7 Mezze Linguine",
              "tipo": "lunga",
              "cottura": 11
          },
          {
              "id": 4,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "n.11 Spaghettino Quadrato",
              "tipo": "lunga",
              "cottura": 9
          },
          {
              "id": 5,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.38 Mezze maniche",
              "tipo": "corta",
              "cottura": 12
          },
          {
              "id": 6,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.44 Sedani",
              "tipo": "corta",
              "cottura": 8
          },
          {
              "id": 7,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.49 Sedanini",
              "tipo": "corta",
              "cottura": 8
          },
          {
              "id": 8,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.53 Lumachine",
              "tipo": "corta",
              "cottura": 12
          },
          {
              "id": 9,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.55 Chifferi rigati",
              "tipo": "corta",
              "cottura": 12
          },
          {
              "id": 10,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.58 Misto corto",
              "tipo": "corta",
              "cottura": 9
          },
          {
              "id": 11,
              "src": "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
              "titolo": "N.84 Ditale Quadrato",
              "tipo": "cortissima",
              "cottura": 12
          }
      ]
    }
  } 
}
</script>

<style lang="scss">
// importare il nostro scss generico.
@import "./style/app.scss"

</style>
