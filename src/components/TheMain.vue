<template>
    <div class="container jumbotron-2">

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



    <div class="bg-primary p-5 d-flex align-items-center gap-3">

        <div class="card-icon d-flex align-items-center gap-3" v-for="icona in banners">
            <img :src="icona.icon" alt="" srcset="">
            <small class="text-white">{{ icona.name }}</small>

        </div>

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
import { itemsBanners } from "../composaples/arrayIcons";
export default {
    data() {
        return {
            listaFumetti: dcHeroes,
            banners: itemsBanners,
        }
    },
}


</script>

<style lang="scss" scoped>
.container-fluid {
    background-color: black;
}

.card {
    border: none;
}

.jumbotron {
    background-image: url(/footer-bg.jpg);
    height: 400px;
    background-repeat: no-repeat;
    background-position: center top;
    width: 100%;
    color: white;
    background-size: cover;

}

.img {
    width: 30px;
    height: 30px;
}

.card-icon {
    width: fit-content;
    img {width: 35px ;}
}

.jumbotron-2 {
    background-image: url(/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center top;
    width: 100%;
    height: 300px;
}
</style>