<template>
    <header class="bar">
        <div>
            <img src="../assets/img/dc-logo.png" alt="DC Logo">
        </div>
        <div>
            <ul>
                <li :key="index" v-for="link,index in links">{{link}}</li>
            </ul>
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
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: auto;
        padding: 30px 0;

        div {
            width: 50%;
        }

        ul {
            display: flex;
            justify-content: space-between;
            list-style: none;
        }
    }
</style>