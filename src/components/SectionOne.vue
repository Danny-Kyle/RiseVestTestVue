<template>
    <main class="h">
        <div class="texts">
            <span>Dollar investments that help you grow</span>
            <p>We put your money in high quality assets that help you build wealth and achieve your financial goals.</p>

            <div class="images">
                <img src="@/assets/appstore.png"  alt="appstore">
                <img src="@/assets/playstore.png" alt="playstore">
            </div>
        </div>
        <div class="img">
            <img src="@/assets/phone.svg" alt="phone">
        </div>
    </main>
</template>

<script>

</script>

<style scoped>
.h {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-bottom: 10px;
}

.texts span{
    color: #07969E;
    letter-spacing: -2px;
    font-size: 36px;
    font-weight: 600;
    
}

.images {
    display: flex;
    flex-direction: row;
    gap: 10px;
}

@media (min-width: 1280px) {
    .h {
        display: flex;
    flex-direction: row;
    justify-content: space-between;
    }
    .texts span{
    color: #07969E;
    letter-spacing: -2px;
    font-size: 56px;
    font-weight: 600;
}
}

</style>