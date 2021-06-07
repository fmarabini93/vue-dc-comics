<template>
    <div class="bar">
        <div class="container">
            <div>
                <button class="uppercase">Sign-Up Now!</button>
            </div>
            <div>
                <ul>
                    <li class="uppercase"><a href="#">Follow Us</a></li>
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
        font-weight: bold;

        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            button {
                padding: 15px;
                border: 2px solid #0282f9;
                font-size: 18px;
                font-weight: bold;
                color: white;
                background-color: #303030;
            }

            ul {
                display: flex;
                justify-content: space-between;
                align-items: center;
                list-style: none;

                li {
                    padding: 0 10px;

                    a {
                        text-decoration: none;

                        &:first-child {
                            color: #0282f9;
                        }
                    }
                }
            }
        }
    }
</style>