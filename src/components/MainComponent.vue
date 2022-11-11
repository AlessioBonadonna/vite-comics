<template>
    <main>
        <section>
            <div class="container-start">
                <button><a href="#nogo"> current series </a> </button>
                <h2> --> Contenctgoes Here &lt;-- </h2>

            </div>

        </section>

    </main>
</template>

<script>
export default {
    name: 'MainComponent'

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

main {
    color: $whitetext;
    background-color: $blacktext;
}

section {
    @include dflex;
    @include container;
    background-color: $blacktext;
    height: 15vh;

    button {
        position: absolute;
        top: -50px;
        left: 0;
        background-color: $bluelink;
        height: 40px;
        padding: 10px;
        border: none;

        a {
            text-transform: uppercase;
            color: $whitetext;
            font-size: 1.2em;
            text-decoration: none;
            font-weight: bold;
        }
    }



    .container-start {
        max-width: 1170px;
        padding: 1rem;
        position: relative;

        justify-content: flex-start;



        h2 {
            color: $whitetext;
        }
    }
}
</style>