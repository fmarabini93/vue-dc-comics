<template>
    <div class="bar">
        <div class="container">
            <div>
                <button>Sign-Up Now!</button>
            </div>
            <div>
                <ul>
                    <li><a href="#">Follow Us</a></li>
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="Twitter"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="Youtube"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Periscope"></a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .bar {
        justify-content: space-between;
        background-color: #303030;

        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            ul {
                display: flex;
                justify-content: space-between;
                align-items: center;
                list-style: none;

                li {
                    padding: 0 10px;
                }
            }
        }
    }
</style>