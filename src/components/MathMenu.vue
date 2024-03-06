<template>
    <div class="container-operation-picker">
        <div class="operation-picker">
            <button class="operation-btn">
                Multiplication
            </button>
            <button class="operation-btn">
                Division
            </button>
            <button class="operation-btn">
                Square Root
            </button>
            <button class="operation-btn">
                Factorization
            </button>
            <button class="operation-btn">
                Mean
            </button>
            <button class="operation-btn">
                Mode
            </button>
            <button class="operation-btn">
                Median
            </button>
            <button class="operation-btn">
                First Degree Equation
            </button>
            <button class="operation-btn">
                Second Degree Equation
            </button>
            <button class="operation-btn">
                Trigonometry
            </button>
            <button class="operation-btn">
                Proportional Quantities
            </button>
            <button class="operation-btn">
                Probability
            </button>
            <button class="operation-btn">
                Something
            </button>
        </div>
    </div>

</template>
<script lang="ts">
console.log("Math menu")


export default {}
</script>
<style scoped lang="css">
    .container-operation-picker {
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .operation-picker {
        width: 50%;
        /*background: #8B8C89;*/
        background: #8DA9C4;
        min-height: 500px;
        border-radius: 10px;
        height: auto;
        justify-content: center;
        align-items: center;
        display: grid;
        grid-template-columns: repeat(auto-fill, 210px);
        grid-row-gap: 10px;
        padding: 20px 0px 20px 0px;
    }

    .operation-btn {
        width: 200px;
        height: 200px;
        background: #134074;
        border-radius: 10px;
        border: 2px solid #fff;
        color: #fff;
        font-size: 24px;
    }

    .operation-btn:hover {
        cursor: pointer;
    }
</style>