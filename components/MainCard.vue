<template>
    <div class="card pt-8 pb-6" >
      <div class="relative z-10 pl-6">
            <h1 class="title">Qoraqalpog'iston R</h1>
        <div class="mt-7">
            <p class="info">Xayriya qilganlar soni: 150</p>
            <p class="info">Ekilgan daraxtlar soni: 360</p>
            <p class="info">Ekilayotgan  daraxtlar soni: 245</p>

        </div>
      </div>
    </div>
</template>
<style scoped>
    .card{
        position: relative ;
        background: linear-gradient(180deg, rgba(28, 43, 39, 0.8) 0%, #1C2B27 100%);
        border: 1px solid #A5ABAA;
        box-sizing: border-box;
        border-radius: 16px;
        width: 283px;
        height: 190px;
        background-image: url(../static/main/nukus.png);
        color: #fff;
    }
    .card::before{
        content: "";
        position: absolute;
        background: linear-gradient(180deg, rgba(28, 43, 39, 0.8) 0%, #1C2B27 100%);
        border: 1px solid #A5ABAA;
        box-sizing: border-box;
        border-radius: 16px;
         width: 283px;
        height: 190px;
        top: 0;
    }
    .title{
        font-weight: 700;
        font-size: 24px;
        line-height: 30px;
    }
</style>