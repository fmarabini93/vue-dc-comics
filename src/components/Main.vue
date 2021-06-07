<template>
    <div>
        <div id="main-top" class="bar">
            <div class="container">
                <h1>-->Content goes here</h1>
            </div>
        </div>
        <div id="main-center" class="bar">
            <div class="container">
                <ul>
                    <li><img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">Digital Comics</li>
                    <li><img src="../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">DC Merchandise</li>
                    <li><img src="../assets/img/buy-comics-subscriptions.png" alt="Subscription">Subscription</li>
                    <li><img src="../assets/img/buy-comics-shop-locator.png" alt="Comics Shop Locator">Comic Shop Locator</li>
                    <li><img src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">DC Power Visa</li>
                </ul>
            </div>
        </div>
        <div id="main-bottom">
            <div class="container">
                <div>

                </div>
                <div>
                    <img src="../assets/img/dc-logo-bg.png" alt="DC Background Logo">
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #main-top {
        line-height: 150px;
        color: white;
        background-color: black;
    }

    #main-center {
        display: flex;
        align-items: center;
        padding: 30px 0;
        color: white;
        background-color: #0282f9;

        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;
            list-style: none;

            li {
                width: 20%;
                display: flex;
                align-items: center;
            }
        }

        img {
            height: 60px;
            padding-right: 20px;
        }
    }

    #main-bottom {
        height: 375px;
        overflow: hidden;
        background-image: url(../assets/img/footer-bg.jpg);

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;

            img {
                margin-top: -95px;
            }
        }
    }
</style>