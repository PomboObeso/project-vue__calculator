<template>
    <div class="display">{{value}}</div>
</template>

<script>
export default {
    props: ['value']
}
</script>

<style>
    .display {
        grid-column: span 4;
        background-color: #0009;
        
        display: flex;
        justify-content: flex-end;
        align-items: center;
        padding: 15px;
        font-size: 2.2em;
        overflow: hidden;
    }
</style>