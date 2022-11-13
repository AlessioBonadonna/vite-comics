<template>
    <div class="container">
        <div class="logo">
            <img src="/public/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index" :class="{ 'active': link.current }">
                    <a :href="link.url" :class="{ 'active': link.current }">{{ link.text }}</a>
                </li>
            </ul>
        </nav>

    </div>
</template>

<script>
import { links } from '../data/data';
export default {
    name: 'HeaderComponent',
    data() {
        return {
            links: links
        }
    }

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.container {
    @include dflex;

}

ul {
    @include dflex;

    li {
        margin-right: 10px;
        list-style: none;
        text-transform: uppercase;

        font-size: 1em;


        a {
            text-decoration: none;
            color: $blacktext;
            height: 50px;
            padding-bottom: 50px;

            &.active,
            &:hover,
            &:active {
                color: $bluelink;
                border-bottom: 5px solid $bluelink;
            }


        }
    }

}
</style>