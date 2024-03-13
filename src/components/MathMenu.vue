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
        </div>
    </div>

</template>
<script lang="ts">
console.log("Math menu")
import { ref } from 'vue';


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
                },
                {
                    title: 'Square Root',
                    icon: '√',
                    link: '/sqrt'
                },
                {
                    title: 'Factorization',
                    icon: 'a² - b²',
                    link: '/factorization'
                },
                {
                    title: 'Mean',
                    icon: 'x1 + xn / xn',
                    link: '/mean'
                },
                {
                    title: 'Mode',
                    icon: 'x1 + x2 + x2 + x3',
                    link: '/mode'
                },
                {
                    title: 'Median',
                    icon: 'x1 + x2 + x3',
                    link: '/mode'
                },
                {
                    title: 'First Degree Equation',
                    icon: 'ax + b = c',
                    link: '/firstdegreeq'
                },
                {
                    title: 'Second Degree Equation',
                    icon: 'ax² + bx + c = 0',
                    link: '/secdegreeq'
                },
                {
                    title: 'Trigonometry',
                    icon: 'θ',
                    link: '/trigonometry'
                },
                {
                    title: 'Proportional Quantities',
                    icon: 'y = x',
                    link: '/proportionalq'
                },
                {
                    title: 'Probability',
                    icon: '%',
                    link: '/probability'
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
        height: 180px;
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
        height: 95px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .operation-btn:hover {
        cursor: pointer;
    }
</style>