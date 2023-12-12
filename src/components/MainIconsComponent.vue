<script>
export default {
    name: 'IconsComponent',
    data() {
        return {
            icons: [
                {
                    name: 'digital comics',
                    icon: '/img/buy-comics-digital-comics.png',
                    link: '#'
                },
                {
                    name: 'dc merchandise',
                    icon: '/img/buy-comics-merchandise.png',
                    link: '#'
                },
                {
                    name: 'subscription',
                    icon: '/img/buy-comics-subscriptions.png',
                    link: '#'
                },
                {
                    name: 'comis shop locator',
                    icon: '/img/buy-comics-shop-locator.png',
                    link: '#'
                },
                {
                    name: 'dc power visa',
                    icon: '/img/buy-dc-power-visa.svg',
                    link: '#'
                },
            ]
        }
    }
}
</script>

<template>
    <div class="icons">
        <div class="container">
            <ul>
                <li v-for="icon in icons">
                    <a :href="icon.link">
                        <img :src="icon.icon" :alt="icon.name">
                        <p>{{ icon.name }}</p>
                    </a>
                </li>
            </ul>

        </div>

    </div>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

.icons {
    background-color: $primarycolor;

    ul {
        display: flex;
        justify-content: space-around;
        padding: 50px 0;
        text-transform: uppercase;
        font-size: 14px;

        li {
            display: flex;
            align-items: center;

            a {
                display: flex;
                align-items: center;
                color: #ffff;
                gap: 15px;

                img {
                    width: 50px;
                }
            }
        }


    }

}
</style>