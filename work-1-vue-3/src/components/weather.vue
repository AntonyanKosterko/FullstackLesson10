<template>
    <html>

    <head>
    <meta charset="UTF-8">
    <title>Informer</title>
    <link rel="stylesheet" href="style.css">
    </head>

    <body>

    <div class="app">
        <div class="informer-container">

        <div class="temperature">
            <img src="img/thermometer.png">
            <div class="temp-real">1</div>
            <div class="temp-feel">-3.8</div>
        </div>

        <div class="flex-break"></div>

        <div class="humidity">
            <img src="../../img/humidity.png"> 12 <small>%</small>
        </div>

        <div class="vertical-divider"></div>

        <div class="wind">
            <img src="../../img/wind.png"> 12 <small>м/с</small>
        </div>

        </div>
    </div>

    </body>

    </html>
</template>

<script>
export default{
  name: 'FirstComponent',
  data(){
    return {text: 'Я новый компонент!'}
  }
}
</script>

<style scoped>
    body {
        margin: 0;
        padding: 0;
        }

        .app {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
        background: rgb(244, 123, 186);
        background: linear-gradient(-25deg, rgba(244, 123, 186, 0.5) 20%, rgba(90, 95, 245, 0.5) 80%);
        }

        .informer-container {
        display: flex;
        align-items: flex-start;
        justify-content: space-between;
        flex-wrap: wrap;
        width: 400px;
        padding: 30px;
        background-image: url('../../img/forest.png');
        background-size: cover;
        background-position: center center;
        border-radius: 20px;
        box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
        }

        .temperature {
        display: flex;
        align-items: flex-end;
        margin: 15px;
        }
</style>
