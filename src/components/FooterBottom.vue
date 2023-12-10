<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            socialList: [
                {
                    name: 'Facebook',
                    icon: '/img/footer-facebook.png',
                    link: '#'
                },
                {
                    name: 'Twitter',
                    icon: '/img/footer-twitter.png',
                    link: '#'
                },
                {
                    name: 'Youtube',
                    icon: '/img/footer-youtube.png',
                    link: '#'
                },
                {
                    name: 'Pinterest',
                    icon: '/img/footer-pinterest.png',
                    link: '#'
                },
                {
                    name: 'Periscope',
                    icon: '/img/footer-periscope.png',
                    link: '#'
                },
            ]
        }
    }
}
</script>

<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="left-side">
                <button>sign-up now!</button>
            </div>
            <div class="right-side">
                <h5>Follow us</h5>
                <ul>
                    <li v-for="social in socialList">
                        <a :href="social.link">
                            <img :src="social.icon" alt="social.name">
                        </a>
                    </li>
                </ul>
            </div>
        </div>

    </div>
</template>

<style lang="scss">
@use '../styles/variables.scss' as *;

.footer-bottom {
    background-color: $footerbgcolor;
    height: 100px;

    .container {
        display: flex;
        justify-content: space-between;

        .left-side {
            padding-top: 30px;

            button {
                padding: 15px;
                text-transform: uppercase;
                color: #ffff;
                background-color: inherit;
                border: 2px solid $primarycolor;
                font-weight: bold;
            }
        }

        .right-side {
            display: flex;
            align-items: center;
            padding-top: 30px;
            text-transform: uppercase;
            color: $primarycolor;
            font-size: 18px;    

            ul {
                display: flex;
                gap: 15px;
                margin-left: 20px;
            }
        }
    }
}
</style>