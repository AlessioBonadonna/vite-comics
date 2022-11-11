<template>
    <main>
        <section>
            <div class="container-start">

                <div class="row">

                    <div class="card" v-for="(comic, index) in comics" :key="index">
                        <div class="imgbox">
                            <img :src="comic.thumb" :alt="comic.series">
                        </div>
                        <div>
                            <h4>{{ comic.series }}</h4>

                        </div>
                    </div>


                </div>

            </div>

        </section>
        <div class="btn">
            <button>load more</button>
        </div>

    </main>
</template>

<script>
import { comics } from '../data/data';
export default {
    name: 'MainComponent',
    data() {
        return {
            comics: comics
        }
    }



}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

main {

    color: $whitetext;
    background-color: $blacktext;
    padding-bottom: 20px;

    section {
        @include dflex;
        @include container;
        background-color: $blacktext;






        .container-start {
            max-width: 1170px;
            padding: 1rem;
            display: flex;
            justify-content: flex-start;

            .row {

                display: flex;
                flex-flow: row wrap;



                .card {
                    // @include dflex;
                    height: 210px;
                    padding: 10px;
                    width: calc(100% / 6);

                    .imgbox {
                        height: 90%;
                        overflow-y: hidden;

                        img {
                            width: 90;

                        }


                    }

                    div {
                        h4 {
                            text-align: center;
                        }
                    }



                }




                h2 {
                    color: $whitetext;
                }
            }
        }




    }

    .btn {

        text-align: center;
        margin-bottom: 10px;

        button {
            background-color: $bluelink;
            height: 40px;
            width: 150px;
            padding: 10px;
            border: none;
            margin-bottom: 10px;
            text-transform: uppercase;
            font-weight: bold;
            color: $whitetext;
            font-size: 1.2em;

            &:hover {
                background-color: black;
                border: 3px solid $bluelink;
                padding: 10px;
            }
        }
    }
}
</style>