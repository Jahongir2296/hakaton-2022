<template>
    <div class="statistika py-16">
        <div class="container">
            <div class="flex justify-between">
                <h1 class="card-title mb-5">Statistika</h1>
                <p class="flex gap-2 items-center cursor-pointer">Hududlar bo'yicha natijalar 
                    <svg width="8" height="14" viewBox="0 0 8 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M0.292893 13.7071C0.683417 14.0976 1.31658 14.0976 1.70711 13.7071L7.70711 7.70711C8.09763 7.31658 8.09763 6.68342 7.70711 6.29289L1.70711 0.292893C1.31658 -0.0976315 0.683417 -0.0976315 0.292893 0.292893C-0.0976311 0.683417 -0.0976311 1.31658 0.292893 1.70711L5.58579 7L0.292893 12.2929C-0.0976311 12.6834 -0.0976311 13.3166 0.292893 13.7071Z" fill="#C0C4C3"/>
                    </svg>
                </p>
            </div>
            <div class="flex gap-5">
                <div class="card relative text-center align-middle">
                    <h2 class="statistica-number">40 mln</h2>
                    <p class="statistica-info">Xayriya qilganlar soni</p>
                    <img class="absolute top-0 right-0" src="../static/statistica/bg-img.png" alt="">
                </div>
                 <div class="card relative text-center align-middle">
                    <h2 class="statistica-number">654 618</h2>
                    <p class="statistica-info">Xayriya qilingan daraxtlar soni</p>
                    <img class="absolute top-0 right-0" src="../static/statistica/bg-img.png" alt="">
                </div>
                 <div class="card relative text-center align-middle">
                    <h2 class="statistica-number">328</h2>
                    <p class="statistica-info">Ekilgan daraxtlar soni</p>
                    <img class="absolute top-0 right-0" src="../static/statistica/bg-img.png" alt="">
                </div>
                 <div class="card relative text-center align-middle">
                    <h2 class="statistica-number">400</h2>
                    <p class="statistica-info">Ekilayotgan  daraxtlar soni</p>
                    <img class="absolute top-0 right-0" src="../static/statistica/bg-img.png" alt="">
                </div>
                
            </div>
        </div>
    </div>
</template>
<style scoped>
    .statistika{
        background: #1C2B27;
        color: #fff;
    }
    .card{
        padding: 50px 23px;
        width: 283px;
        height: 186px;
        background: #1C2B27;
        border: 1px solid #A5ABAA;
        box-sizing: border-box;
        border-radius: 16px;
        
    }
    .card-title{
        font-weight: 700;
        font-size: 36px;
        line-height: 45px;
    }
    .statistica-number{
        font-weight: 700;
        font-size: 36px;
        line-height: 45px;
    }
    .statistica-info{
        font-weight: 500;
        font-size: 24px;
        line-height: 30px;
        color: #C0C4C3;
    }
</style>