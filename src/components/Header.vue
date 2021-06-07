<template>
    <header class="bar">
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <div>
                <ul>
                    <li :key="index" v-for="link,index in links" class="uppercase">{{link}}</li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        data: function() {
            return {
                links: ["Characters","Comics","Movies","TV","Games","Collectibles","Videos","Fans","News","Shop"]
            }
        }
    }
</script>


<style lang="scss" scoped>
    header {
        padding: 30px 0;

        div:not(.container) {
            width: 50%;
        }

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        ul {
            display: flex;
            justify-content: space-between;
            list-style: none;

            li {
                font-size: 14px;
                font-weight: bold;
            }
        }
    }
</style>