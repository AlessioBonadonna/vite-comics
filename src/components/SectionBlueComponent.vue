<template>
    <section class="blue">
        <div class="container">
            <ul>
                <li v-for="(img, index) in blueimg" :key="index">
                    <a :href="img.url">
                        <img :src="img.img" alt="img.text">
                        <span>
                            {{ img.text }}
                        </span>

                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SectionBlueComponent',

    data() {
        return {
            blueimg: [
                {
                    url: "#nogo",
                    img: "/public/img/buy-comics-digital-comics.png",
                    text: "Digital Comics"
                },
                {
                    url: "#nogo",
                    img: "/public/img/buy-comics-merchandise.png",
                    text: "Dc Merchandise"
                },
                {
                    url: "#nogo",
                    img: "/public/img/buy-comics-subscriptions.png",
                    text: "Subscriptions"
                },
                {
                    url: "#nogo",
                    img: "/public/img/buy-comics-shop-locator.png",
                    text: "Comics Shop locator"
                },

                {
                    url: "#nogo",
                    img: "/public/img/buy-dc-power-visa.svg",
                    text: "Dc power Visa"
                }
            ]

        }
    }
}

</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.blue {
    background-color: $bluelink;

    .container {
        padding-top: 40px;
        padding-bottom: 40px;

        ul {
            @include dflex;

            li {
                list-style: none;

                a {
                    @include dflex;
                    color: $whitetext;
                    text-decoration: none;

                    img {
                        width: 50px;


                    }

                    span {
                        margin-left: 8px;
                        text-transform: uppercase;
                    }
                }
            }
        }
    }
}
</style>