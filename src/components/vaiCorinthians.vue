<script setup>
</script>
<template>
    <div class="imagens">
        <div class="triste">
            <p>eu sem vc triste capenga xoxo mofino <span>⬇️</span></p>
            <img src="@/assets/images/triste.jpeg" alt="">
        </div>
        <div class="feliz">
            <p>eu com vc bem feliz da vida <span>⬇️</span></p>
            <img src="@/assets/images/feliz.jpeg" alt="">
        </div>
    </div>
</template>
<style scoped>
    .imagens {
        justify-content: center;
        align-items: center;
        margin-left: 50px;
    }
    .triste {
        margin-bottom: 300px;
        
        width: 300px;
        height: 300px;
    }
    .feliz {
        width: 300px;
        height: 300px;
    }
    img {
        margin-top: 40px;
        width: 100%;
        height: 100%;
       
    }
    p {
        margin: 40px;
        text-align: center;
        font-size: 20px;
        font-weight: bold;
        color: black;
    }
</style>