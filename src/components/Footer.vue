<template>
    <div class="footer-container container">

        <!-- div con logo -->
        <div class="logo-container">
            <img src="../assets/la-molisana-logo.png" />
        </div>

        <!-- div con due ul (menu del footer) -->
        <div class="menu-container">
            <ul>
                <li>Pastificio</li>
                <li><a href="#">Il pastificio</a></li>
                <li><a href="#">Grano decorticato a pietra</a></li>
                <li><a href="#">Filiera Integrata</a></li>
                <li><a href="#">100 anni di pasta</a></li>
                <li><a href="#">Sartoria della pasta</a></li>
            </ul>

            <ul>
                <li>Prodotti</li>
                <li><a href="#">Le Classiche</a></li>
                <li><a href="#">Le Integrali</a></li>
                <li><a href="#">Le Speciali</a></li>
                <li><a href="#">Le Biologiche</a></li>
                <li><a href="#">Le Gluten-Free</a></li>
            </ul>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>

    .footer-container {
        margin-top: 50px;
        display: flex;

        .logo-container {
            width: 40%;
        }

        .menu-container {
            flex-grow: 1;
            display: flex;

            ul {
                width: 50%;
                list-style: none;

                li {
                    font-size: 12px;
                    margin: 5px 0;

                    &:first-child {
                        font-size: 18px;
                        font-weight: bold;
                    }

                    a {
                        color: #333;
                        text-decoration: none;

                        &:hover {
                            text-decoration: underline;
                        } 

                    }


                }


            }


        }

    }

</style>