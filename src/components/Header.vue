<template>
    <div class="header-full">
        <div class="logo-container">
            <img src="../assets/la-molisana-logo.png" />
        </div>
        <nav>
            <ul>
                <li>Home</li>
                <li>Prodotti</li>
                <li>Chi Siamo</li>
                <li>Contatti</li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'Header'
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

                }

            }

        }


    }



</style>
