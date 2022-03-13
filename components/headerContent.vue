<template>
    <div class="container relative z-10">
        <h1 class="header-title m-45">
            Kelajak uchun daraxtlar ekilishiga o'z hissangizni qo'shing!
        </h1>
        <p class="header-info">1ta daraxt 10 000 so'mdan</p>
        <router-link to="/">
            <button class="header-btn">Daraxt ekish</button>
        </router-link>
    </div>
</template>

<style scoped>
.header-title{
    max-width: 586px;
    font-weight: 700;
    font-size: 36px;
    line-height: 45px;
    font-feature-settings: 'pnum' on, 'lnum' on;
    color: #FFFFFF;
    margin-top: 174px;
}
.header-info{
    font-weight: 400;
    font-size: 24px;
    line-height: 30px;
    color: #FFFFFF;
    margin-top:6px ;
}
.header-btn{
    background: #FFFFFF;
    border-radius: 8px;
    padding: 12px 46px;
    margin-top: 16px;
}
</style>
