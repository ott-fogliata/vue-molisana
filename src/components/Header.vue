<template>
    <div class="header-full">
        <div class="logo-container">
            <img src="../assets/la-molisana-logo.png" />
        </div>
        <nav>
            <ul>
                <!-- 
                    la :key serve a vuejs per identificare
                    l'elemento in maniera univoca.
                    Quindi gli attribuiamo un valore 
                    univoco.
                -->
                <li v-for="element in navList" :key="element.id">
                    <a :href="element.link">{{element.name}}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>
              /* 'Home',
                'Prodotti',
                'Chi Siamo',
                'Contatti'*/

export default {
    name: 'Header',
    // Il componente ascolta/recepisce la prop di nome nav.
    /*props: [
        'navList',
    ],*/
    props: {
        // k= nome prop, v=il tipo della prop (String, Array, Object,...)
        navList: Array
    },
    /*
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
            ]
        }
    } 
    */
}
</script>

<style lang="scss" scoped>

    @import "../style/colors.scss";

    .header-full {

        .logo-container {
            text-align: center;
        }

        nav {

            ul {
                display: flex;
                list-style: none;
                justify-content: center;
                font-size: 14px;
                font-weight: bold;

                li {
                    height: 50px;
                    line-height: 50px;
                    padding: 0 10px;
                    cursor: pointer;

                    &:hover {
                        background: $bg-color;
                    }

                    a { 
                        color: #000;
                        text-decoration: none;
                    }

                }

            }

        }


    }



</style>
