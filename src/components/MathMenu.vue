<template>
    <div class="container-operation-picker">
        <div class="operation-picker">
            <button v-for="operation in operations" class="operation-btn">
                <div class="icon-container">
                    {{ operation.icon }}
                </div>
                <div class="subtitle">
                    {{ operation.title }}
                </div>
            </button>

            <!--<button class="operation-btn">
                <div class="icon-container">
                    X
                </div>
                <div class="subtitle">
                    Multiplication
                </div>
            </button>-->
            <!--<button class="operation-btn">
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
            </button>-->
        </div>
    </div>

</template>
<script>
console.log("Math menu")
import { ref } from 'vue';

/*const operations = ref([
    {
        title: 'Multiplication',
        icon: 'X',
        link: '/multiplication'
    },
    {
        title: 'Division',
        icon: '÷',
        link: '/division'
    }
])**/


export default {
    data() {
        return {
            name: 'MathMenu',
            operations: [
                {
                    title: 'Multiplication',
                    icon: 'X',
                    link: '/multiplication'
                },
                {
                    title: 'Division',
                    icon: '÷',
                    link: '/division'
                }
            ]
        }
    }
} 

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
        /*background: #8DA9C4;*/
        /*border: 2px solid #dadada;*/
        min-height: 500px;
        border-radius: 10px;
        height: auto;
        justify-content: center;
        align-items: center;
        display: grid;
        grid-template-columns: repeat(auto-fill, 210px);
        grid-row-gap: 15px;
        padding: 20px 0px 20px 0px;
    }

    .operation-btn {
        width: 200px;
        height: 140px;
        /*background: #134074;*/
        /*background: #76ABAE;*/
        background: transparent;
        border-radius: 10px;
        border: 2px solid #76ABAE;
        color: #76ABAE;
        font-size: 24px;
    }

    .icon-container {
        height: 60px;
        border-bottom: 1px solid #76ABAE;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .subtitle {
        height: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .operation-btn:hover {
        cursor: pointer;
    }
</style>