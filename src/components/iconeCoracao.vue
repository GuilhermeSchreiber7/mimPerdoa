<script setup>
</script>
<template>
    <div class="heart">
        <p>mim perdoa</p>
    </div>
</template>
<style scoped>
    body {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .heart {
        position: relative;
        width: 200px; /* doubled the width */
        height: 190px; /* doubled the height */
        margin: 100px auto 0;
    }

    .heart::before, .heart::after {
        content: '';
        position: absolute;
        width: 100px; /* doubled the width */
        height: 160px; /* doubled the height */
        background-color: red;
        border-radius: 100px 100px 0; /* doubled the border radius */
        transform: rotate(-45deg);
        transform-origin: 0 100%;
        left: 100px; /* doubled the left position */
        top: 0;
    }

    .heart::after {
        left: 0;
        transform: rotate(45deg);
        transform-origin: 100% 100%;
    }
    .heart p {
        position: absolute;
        top: 30%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        font-size: 15px;
        font-weight: bold;
        z-index: 10;
    }
    @keyframes beat {
        0% {
            transform: scale(1);
        }
        25% {
            transform: scale(1.4);
        }
        50% {
            transform: scale(1);
        }
        75% {
            transform: scale(1.4);
        }
        100% {
            transform: scale(1);
        }
    }

    .heart {
        animation: beat 1s infinite;
    }
</style>