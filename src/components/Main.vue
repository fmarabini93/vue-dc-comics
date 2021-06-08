<template>
    <div>
        <div id="main-top">
            <div id="jumbotron"></div>
            <div class="container">
                <button>Current Series</button>
                <div v-for="poster,index in posters" :key="index" class="card"><img :src=poster.thumb alt="#"><h3>{{poster.series}}</h3></div>
                <button class="btm-button">Load More</button>
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
                sites: ["DC","Mad Magazine","DC Kids","DC Universe","DC Power Visa"],
                posters: [
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                    },
                    {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    #main-top {
        line-height: 150px;
        color: white;
        background-color: black;

        .container {
            display:flex;
            justify-content: space-between;
            flex-wrap: wrap;
            position: relative;

            button {
                padding: 5px 20px;
                border: none;
                color: white;
                text-transform: uppercase;
                font-size: 16px;
                font-weight: bold;
                background-color: #0c7cec;
            }

            button:not(.btm-button) {
                position: absolute;
                top: -15px;
            }

            .btm-button {
                position: relative;
                left: 50%;
                transform: translateX(-50%);
                margin-bottom: 20px;
                padding: 10px 40px;
            }

            .card {
                width: calc(100% / 6);
                padding: 50px 0;
                line-height: 20px;
                font-size: 14px;

                h3 {
                    padding-top: 20px;
                    text-transform: uppercase;
                    font-weight: normal;
                }
            }
        }
    }

    #jumbotron {
        height: 375px;
        background-image: url(../assets/img/jumbotron.jpg);
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
                font-size: 14px;
            }
        }

        img {
            height: 50px;
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