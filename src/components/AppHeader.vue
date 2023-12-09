<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            menu: [
                {
                    name: 'characters',
                    link: '#',
                },
                {
                    name: 'comics',
                    link: '#',
                },
                {
                    name: 'movies',
                    link: '#',
                },
                {
                    name: 'tv',
                    link: '#',
                },
                {
                    name: 'games',
                    link: '#',
                },
                {
                    name: 'collectibles',
                    link: '#',
                },
                {
                    name: 'videos',
                    link: '#',
                },
                {
                    name: 'fans',
                    link: '#',
                },
                {
                    name: 'news',
                    link: '#',
                },
                {
                    name: 'shop',
                    link: '#',
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo-container">
                <img src="/img/dc-logo.png" alt="logo">
            </div>
            <ul>
                <li v-for="item in menu">
                    <a :href="menu.link">{{ item.name }}</a>
                </li>
            </ul>
        </div>

    </header>
</template>

<style lang="scss">
@use '../styles/variables.scss' as *;

.container {
    display: flex;
    justify-content: space-between;
    padding: 20px 0;

    img {
        width: 80px;
    }

    ul {
        display: flex;
        align-items: center;
        gap: 30px;
        text-transform: uppercase;

        li {
            height: 100%;
            display: flex;
            align-items: center;
            color: $graytextcolor;

            &:hover {
                color: $primarycolor;
                border-bottom: 5px solid $primarycolor;
            }
        }
    }


}
</style>