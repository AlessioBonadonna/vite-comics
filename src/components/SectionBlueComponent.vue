<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(img, index) in blueimg" :key="index">
                    <a :href="img.url">
                        <img :src="img.img" alt="img.text">
                        <div>
                            <p>{{ img.text }}</p>
                        </div>

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
                    img: "../assets/img/buy-comics-digital-comics.png",
                    text: "Digital Comics"
                },
                {
                    url: "#nogo",
                    img: "../assets/img/buy-comics-merchandise.png",
                    text: "Digital Comics"
                },
                {
                    url: "#nogo",
                    img: "../assets/img/buy-comics-shop-locator.png",
                    text: "Digital Comics"
                },
                {
                    url: "#nogo",
                    img: "../assets/img/buy-comics-subscriptions.png",
                    text: "Digital Comics"
                },
                {
                    url: "#nogo",
                    img: "../assets/img/buy-comics-dc-power-visa.png",
                    text: "Digital Comics"
                }
            ]

        }
    }
}

</script>

<style lang="scss" scoped>

</style>