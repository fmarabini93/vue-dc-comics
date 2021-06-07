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
                    <li class="uppercase"><img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">Digital Comics</li>
                    <li class="uppercase"><img src="../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">DC Merchandise</li>
                    <li class="uppercase"><img src="../assets/img/buy-comics-subscriptions.png" alt="Subscription">Subscription</li>
                    <li class="uppercase"><img src="../assets/img/buy-comics-shop-locator.png" alt="Comics Shop Locator">Comic Shop Locator</li>
                    <li class="uppercase"><img src="../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">DC Power Visa</li>
                </ul>
            </div>
        </div>
        <div id="main-bottom">
            <div class="container">
                <div id="lists" class="clearfix">
                    <div class="float">
                        <h3 class="uppercase">DC Comics</h3>
                        <ul>
                            <li v-for="comic,index in comics" :key="index" class="not-uc">{{comic}}</li>
                        </ul>
                        <h3 class="uppercase">Shop</h3>
                        <ul>
                            <li v-for="shop,index in shops" :key="index" class="not-uc">{{shop}}</li>
                        </ul>
                    </div>
                    <div class="float">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="dc,index in dcs" :key="index" class="not-uc">{{dc}}</li>
                        </ul>
                    </div>
                    <div class="float">
                        <h3 class="uppercase">Sites</h3>
                        <ul>
                            <li v-for="site,index in sites" :key="index" class="not-uc">{{site}}</li>
                        </ul>  
                    </div>
                </div>
                <div>
                    <img src="../assets/img/dc-logo-bg.png" alt="DC Background Logo">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            comics: ["Characters","Comics","Movies","TV","Games","Videos","News"],
            shops: ["Shop DC","Shop DC Collectibles"],
            dcs: ["Terms of Use","Privacy Policy (New)","Ad Choices","Advertising","Jobs","Subscriptions","Talent Workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"],
            sites: ["DC","Mad Magazine","DC Kids","DC Universe","DC Power Visa"]
        }
    }
}
</script>

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
        display: flex;
        align-items: center;
        overflow: hidden;
        color: white;
        background-image: url(../assets/img/footer-bg.jpg);

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        #lists {

            .float {
                padding-right: 40px;

                ul {
                    list-style: none;

                    li {
                        padding: 3px 0;
                        font-size: 14px;
                        color: #959595;
                    }
                }

                h3 {
                    padding: 15px 0;
                }
            }
        }
    }
</style>