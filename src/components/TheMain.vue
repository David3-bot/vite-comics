<template>
    <div class="container-fluid jumbotron-2">
    
    </div>

    <div class="container bg-black p-5">
        <div class="row">
            <div class="col-2" v-for="fumetto in listaFumetti">
                <div class="card ratio ratio-1x1" style="width: 8rem ;">
                    <img :src="fumetto.thumb" class="" alt="">

                </div>
                <div class="card-body">
                    <p class="card-title text-white">{{ fumetto.series }}</p>
                </div>
            </div>

        </div>
    </div>



    <div class="bg-primary d-flex justify-content-around p-5">
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
        <div class="card-icon"><img src="/buy-comics-digital-comics.png" alt="" srcset=""></div>
    </div>
    <section class="jumbotron">

        <div class="container">

            <div class="row">
                <div class="col-10 d-flex">
                    <ul>
                        <h5>DC Comics</h5>
                        <li>characters</li>
                        <li>comics</li>
                        <li>movies</li>
                        <li>tv</li>
                    </ul>
                    <ul>
                        <h5>Shop</h5>
                        <li>gww</li>
                        <li>hthtd</li>
                        <li>shfyjdt</li>
                        <li>sgdfs</li>
                        <li>hgfkhkg</li>
                    </ul>
                    <ul>
                        <h5>DC</h5>
                        <li>rhdfhdt</li>
                        <li>shrdshjdgh</li>
                        <li>sgaere</li>
                        <li>wghdhgh</li>
                        <li>shdezhd</li>
                    </ul>
                    <ul>
                        <h5>Sites</h5>
                        <li>shgsdhgf</li>
                        <li>kukjggh</li>
                        <li>ghdrf</li>
                        <li>jhyjyt</li>
                        <li>dhdfhh</li>
                    </ul>

                </div>
            </div>

        </div>
    </section>
</template>

<script>
import { dcHeroes } from "../../src/composaples/array";
export default {
    data() {
        return {
            listaFumetti: dcHeroes
        }
    },
}


</script>

<style scoped>
.container-fluid {
    background-color: black;
}

.card {
    border: none;
}

.jumbotron {
    background-image: url(/footer-bg.jpg);
    padding-top: 300px;
    padding-right: 300px;
    background-repeat: no-repeat;
    background-position: center top;
    width: 100%;
    color: white;
    background-size: cover;

}

.img {
    width: 30px;
}

.card-icon {
    width: fit-content;
}

.jumbotron-2 {
    background-image: url(/jumbotron.jpg);
    background-repeat: no-repeat;
    background-position: center top;
    width: 100%;
}
</style>