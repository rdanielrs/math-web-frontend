<template>
    <header>
        <div class="header_div">
            <h1>vue-math</h1>
            <div class="nav">
                <a href="#">Home</a>
                <a href="#">About</a>
                <a href="#">Contact</a>
            </div>
        </div>
    </header>
</template>



<script lang="ts">
console.log("Header")

export default {}
</script>



<style lang="css" scoped>

    header {
        /*background: #34568B;*/
        /*background: #274c77;*/
        height: 85px;
        width: 100%;
        top: 0;
        left: 0;
        position: absolute;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .header_div {
        background: #274c77;
        width: 95%;
        height: 75px;
        border-radius: 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0px 10px 0px 10px;
        h1 {
            color: #fff;
            font-family: "Kode Mono", monospace;
        }

    }

    .nav {
        a {
            color: #fff;
            font-size: 20px;
            font-family: "Open Sans", sans-serif;
            padding-left: 10px;
        }
        a:hover {
            background: transparent;
            color: #55c1d1;
        }

    }
</style>