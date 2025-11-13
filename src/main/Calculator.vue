<template>
    <div class="calculator">
        <Display value="1000" />
        <!-- FLAG: Resolvi refatorar o nome da função personalizada para onCalc -->
        <Button label="AC" triple @onCalc="clearMemory" />
        <Button label="/" operation @onCalc="setOperation"/>
        <Button label="7" @onCalc="addDigit" />
        <Button label="8" @onCalc="addDigit" />
        <Button label="9" @onCalc="addDigit" />
        <Button label="*" operation @onCalc="setOperation" />
        <Button label="4" @onCalc="addDigit" />
        <Button label="5" @onCalc="addDigit" />
        <Button label="6" @onCalc="addDigit" />
        <Button label="-" operation @onCalc="setOperation" />
        <Button label="1" @onCalc="addDigit" />
        <Button label="2" @onCalc="addDigit" />
        <Button label="3" @onCalc="addDigit" />
        <Button label="+" operation @onCalc="setOperation" />
        <Button label="0" @onCalc="addDigit" double />
        <Button label="." @onCalc="addDigit" />
        <Button label="=" operation @onCalc="setOperation" />
    </div>
</template>

<script>
import Display from '@/components/Display.vue';
import Button from '@/components/Button.vue';

export default {
    components: {Button, Display},
    methods: {
        clearMemory() {
        },
        setOperation(operation) {
        },
        addDigit(n) {
        }
    }
}
</script>

<style>
    .calculator {
        height: 320px;
        width: 235px;
        border-radius: 5px;
        overflow: hidden;

        display: grid;
        grid-template-columns: repeat(4, 25%);
        grid-template-rows: 1fr 48px 48px 48px 48px 48px;
    }
</style>