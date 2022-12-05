<template>
    <div class="">
        <nav class="Navbar d-flex justify-content-between align-items-center py-3">
            <div>
                <img src="/dc-logo.png" alt="" srcset="">
            </div>

            <div class="">
                <ul class="d-flex">
                    <li class="p-2" v-for="pippo in listaBottoni"><a href="">{{pippo}}</a></li>
                </ul>
            </div>

        </nav>
    </div>
</template>

<script>
import { navBarItems } from "../../src/composaples/arraynav";
export default {
    data() {
        return {
            listaBottoni: navBarItems
        }
    },
}


</script>

<style scoped>
.navbar {
    background-color: white;
}
</style>