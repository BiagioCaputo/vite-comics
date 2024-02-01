<script>
export default {
    name: 'AppBottomFooter',

};
</script>

<template>
    <footer>
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
#bottom-footer {
    background-color: #303030;
    padding: 20px 0;
}

#bottom-footer .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

button {
    background: none;
    border: 2px solid #047EEF;
    padding: 10px 20px;
    color: white;
    cursor: pointer;
}

.icons-box {
    display: flex;
    gap: 15px;
    align-items: center;
}

h2 {
    color: #047EEF;
}

.icons-list {
    display: flex;
    gap: 10px;
}

ul li {
    list-style-type: none;
}

ul li a {
    color: #959595;
}
</style>