<script>
export default {
    name: 'AppFooter',
    data() {
        return {
            dcComics: [
                { ref: '#', name: 'Characters' },
                { ref: '#', name: 'Comics' },
                { ref: '#', name: 'Movies' },
                { ref: '#', name: 'TV' },
                { ref: '#', name: 'Games' },
                { ref: '#', name: 'Videos' },
                { ref: '#', name: 'News' },
            ],
            shop: [
                { ref: '#', name: 'Shop Dc' },
                { ref: '#', name: 'Shop DC collectibles' }
            ],
            dc: [
                { ref: '#', name: 'Terms Of Use' },
                { ref: '#', name: 'Privacy policy (New)' },
                { ref: '#', name: 'Ad Choices' },
                { ref: '#', name: 'Advertising' },
                { ref: '#', name: 'Jobs' },
                { ref: '#', name: 'Subscriptions' },
                { ref: '#', name: 'Talent Workshops' },
                { ref: '#', name: 'CPSC Certificates' },
                { ref: '#', name: 'Ratings' },
                { ref: '#', name: 'Shop Help' },
                { ref: '#', name: 'Contact Us' },
            ],
            sites: [
                { ref: '#', name: 'DC' },
                { ref: '#', name: 'MAD Magazine' },
                { ref: '#', name: 'DC Kids' },
                { ref: '#', name: 'Dc Universe' },
                { ref: '#', name: 'DC Power Visa' },
            ],
        }
    },

};
</script>

<template>
    <footer>
        <div id="upper-footer">
            <div class="container">
                <div class="ul-container">
                    <div class="">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="link of dcComics"><a :href="link.ref">{{ link.name }}</a></li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="link of shop"><a :href="link.ref">{{ link.name }}</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>DC</h3>
                        <ul>
                            <li v-for="link of dc"><a :href="link.ref">{{ link.name }}</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="link of sites"><a :href="link.ref">{{ link.name }}</a></li>
                        </ul>
                    </div>
                </div>
                <div>
                    <figure>
                    </figure>
                </div>
            </div>

        </div>

        <div id="bottom-footer">
            <div class="container">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div class="icons-box">
                    <h2>FOLLOW US</h2>
                    <ul class="icons-list">
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>

                </div>
            </div>

        </div>
    </footer>
</template>


<style scoped>
#upper-footer {
    background-image: url(./../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;

    color: white;
    padding: 30px 0;

    position: relative;
    overflow: hidden;
}

#upper-footer .container {
    display: flex;
    justify-content: space-between;
}

h3 {
    margin-bottom: 20px;
    margin-top: 20px;
}

ul li {
    list-style-type: none;
    line-height: 1.5;
}

ul li a {
    color: #959595;
}

.ul-container {
    display: flex;
    gap: 50px;
}

figure {
    position: absolute;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-size: contain;
    width: 600px;
    height: 600px;
    right: 40px;
    top: -100px;

}

#bottom-footer {
    background-color: #303030;
    padding: 20px 0;
}

#bottom-footer .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#bottom-footer button {
    background: none;
    border: 2px solid #047EEF;
    padding: 10px 20px;
    color: white;
    cursor: pointer;
}

#bottom-footer .icons-box {
    display: flex;
    gap: 15px;
    align-items: center;
}

#bottom-footer h2 {
    color: #047EEF;
}

#bottom-footer .icons-list {
    display: flex;
    gap: 10px;
}

#bottom-footer ul li {
    list-style-type: none;
}

#bottom-footer ul li a {
    color: #959595;
}
</style>