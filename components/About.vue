<template>
    <div class="about">
         <div class="container flex">
            <div>
                <h1 class="title">Loyiha haqida</h1>
                <p class="info mt-4">Ushbu loyiha O'zbekistonning barcha hududlarida daraxt ekish uchun mablag'
                    to'plash va ekish uchun yaratilgan. Loyiha orqali siz chet-davlatdan turib ham O'zbekistonning 
                    hohlagan hududi uchun daraxtlar ekishingiz mumkin bo'ladi. Bu orqali siz kelajak uchun toza havoni 
                    ta'minlashga o'z hissangizni qo'shasiz! 
                </p>
                <button class="btn flex gap-2">Batafsil 
                    <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M6.91076 15.5892C7.2362 15.9146 7.76384 15.9146 8.08928 15.5892L13.0893 10.5892C13.4147 10.2637 13.4147 9.7361 13.0893 9.41066L8.08928 4.41066C7.76384 4.08522 7.2362 4.08522 6.91076 4.41066C6.58533 4.7361 6.58533 5.26374 6.91076 5.58917L11.3215 9.99992L6.91076 14.4107C6.58533 14.7361 6.58533 15.2637 6.91076 15.5892Z" fill="white"/>
                    </svg>
                </button>
            </div>
            <div>
                <img src="../static/about/plants.png" alt="plants">
            </div>
    </div>
    </div>
</template>
<style scoped>
    .about{
       background: #031410;
       padding-top: 58px;
    }
    .title{
        font-weight: 700;
        font-size: 36px;
        line-height: 45px;
        font-feature-settings: 'pnum' on, 'lnum' on;
        color: #FFFFFF;
    }
    .info{
        max-width: 788px;
        font-weight: 400;
        font-size: 24px;
        line-height: 140%;
        font-feature-settings: 'pnum' on, 'lnum' on;
        color: #C0C4C3;
      }
    .btn{
        background: rgba(255, 255, 255, 0.1);
        border-radius: 8px;
        padding: 12px 32px;
        font-weight: 700;
        font-size: 16px;
        line-height: 20px;
        font-feature-settings: 'pnum' on, 'lnum' on;
        color: #FFFFFF;
        margin-top: 17px;
    }  
</style>