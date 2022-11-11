<template>
    <div class="hero">
        <button><a href="#nogo">current series</a> </button>
    </div>
</template>

<script>
export default {
    name: 'JumboComponent'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.hero {
    background-image: url(../../public/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 40vh;
    position: relative;

    button {
        position: absolute;
        bottom: -20px;
        left: 210px;
        background-color: $bluelink;
        height: 40px;
        padding: 10px;
        border: none;
        color: white;
        margin-top: 10px;
        ;

        a {
            text-transform: uppercase;
            color: $whitetext;
            font-size: 1.2em;
            text-decoration: none;
            font-weight: bold;
        }
    }
}
</style>