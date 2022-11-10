<template>
    <main>
        <section>
            <div class="container-start">
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



    .container-start {
        max-width: 1170px;
        padding: 1rem;

        justify-content: flex-start;

        h2 {
            color: $whitetext;
        }
    }
}
</style>