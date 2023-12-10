<script>
export default {
    name: 'FooterTop',
    data() {
        return {
            menu: [
                {
                    name: 'Dc comics',
                    items: [
                        {
                            text: 'Characters',
                            link: '#'
                        },
                        {
                            text: 'Comics',
                            link: '#'
                        },
                        {
                            text: 'Movies',
                            link: '#'
                        },
                        {
                            text: 'TV',
                            link: '#'
                        },
                        {
                            text: 'Games',
                            link: '#'
                        },
                        {
                            text: 'Videos',
                            link: '#'
                        },
                        {
                            text: 'News',
                            link: '#'
                        },
                    ]

                },
                {
                    name: 'Shop',
                    items: [
                        {
                            text: 'Shop DC',
                            link: '#'
                        },
                        {
                            text: 'Shop DC Collectibles',
                            link: '#'
                        },
                    ]
                },
                {
                    name: 'DC',
                    items: [
                        {
                            text: 'Terms of Use',
                            link: '#'
                        },
                        {
                            text: 'Privacy policy(New)',
                            link: '#'
                        },
                        {
                            text: 'Ad Choices',
                            link: '#'
                        },
                        {
                            text: 'Advertising',
                            link: '#'
                        },
                        {
                            text: 'Jobs',
                            link: '#'
                        },
                        {
                            text: 'Subscriptions',
                            link: '#'
                        },
                        {
                            text: 'Talent Workshops',
                            link: '#'
                        },
                        {
                            text: 'CPSC Certificates',
                            link: '#'
                        },
                        {
                            text: 'Ratings',
                            link: '#'
                        },
                        {
                            text: 'Shop Help',
                            link: '#'
                        },
                        {
                            text: 'Contacts Us',
                            link: '#'
                        },
                    ]
                },
                {
                    name: 'Sites',
                    items: [
                        {
                            text: 'DC',
                            link: '#'
                        },
                        {
                            text: 'MAD Magazine',
                            link: '#'
                        },
                        {
                            text: 'DC Kids',
                            link: '#'
                        },
                        {
                            text: 'DC Universe',
                            link: '#'
                        },
                        {
                            text: 'DC Power Visa',
                            link: '#'
                        },
                    ]
                },

            ]
        }
    }
}
</script>

<template>
    <div class="footer-top">
        <div class="container">
            <div class="lists">
                <div v-for="list in menu">
                    <h4>{{ list.name }}</h4>
                    <ul>
                        <li v-for="item in list.items">
                            <a :href="item.link">{{ item.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="logo-bg">
            
            </div>

        </div>
    </div>
</template>

<style lang="scss">
@use '../styles/variables.scss' as *;

.footer-top {
    background-image: url(/img/footer-bg.jpg);
    background-size: cover;

    .container {
        height: 400px;
        display: flex;
        align-items: center;
        position: relative;

        .lists {
            height: 100%;
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            padding: 30px;
            width: 40%;

            h4 {
                margin: 20px 0;
                text-transform: uppercase;
                color: #ffff;
            }
            li {
                padding: 3px;
                font-size: 13px;
                
                a {
                    color: #959595;
                }
            }
        }

        .logo-bg {
            width: 60%; 
            height: 100%;
            background-image: url(/img/dc-logo-bg.png);
            background-position-y: -100px; 
            background-position: right; 
            background-repeat: no-repeat;
            
        }
    }

}
</style>