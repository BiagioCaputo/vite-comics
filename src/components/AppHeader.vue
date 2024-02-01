<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                { ref: '#', name: 'Characters', current: false },
                { ref: '#', name: 'Comics', current: false, },
                { ref: '#', name: 'Movies', current: false, },
                { ref: '#', name: 'TV', current: false, },
                { ref: '#', name: 'Games', current: false, },
                { ref: '#', name: 'Collectibles', current: false, },
                { ref: '#', name: 'Videos', current: false, },
                { ref: '#', name: 'Fans', current: false, },
                { ref: '#', name: 'News', current: false, },
                { ref: '#', name: 'Shop', current: false, },
            ]
        }
    },
};
</script>

<template>
    <header>
        <nav class="container">

            <figure>
                <img src="../assets/img/dc-logo.png" alt="logo dc">
            </figure>


            <ul>
                <li v-for="link of links"><a :href="link.ref">{{ (link.name).toUpperCase() }}</a></li>
            </ul>

        </nav>
    </header>
</template>

<style scoped>
nav {
    display: flex;
    align-items: center;
    padding: 20px 0;
}

figure {
    width: 40%;
}

ul {
    display: flex;
    gap: 10px;
    width: 60%;
}

ul li {
    list-style-type: none;
}

ul li a {
    font-weight: bold;
    padding: 10px;
    color: #464646;
}

ul li a.active,
ul li a:hover {
    color: #0282F9;
}
</style>