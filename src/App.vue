<template>
    <div id="app">
        <h1>Olá Vue</h1>
    </div>
</template>

<script>
export default {

}
</script>

<style>
@font-face {
    font-family: "RobotoMono" ;
    src: url("./fonts/RobotoMono-Thin.ttf");
}
* {
    font-family: "RobotoMono", monospace;
}

body {
    margin: 0;
    padding: 0;
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;

    color: #fff;
    background: linear-gradient(to right, rgb(82,102, 115), rgb(39, 44, 70));
}
</style>