<template>
   <div class="question ">
       <div class="container">
               <h1 class="title">O'z hududingizga daraxt 
                ekmoqchimisiz?</h1>
    <div class="flex question-content">
        <div>
           <img class="img" src="../static/answer/map.png" alt="">
        </div>
        <div>
            <h2 class="select-title">Qaysi hududga daraxt ekmoqchisiz?</h2>
            <div class="flex gap-4">
                <div>
                    <p class="seleckt-name">Viloyat</p>
                    <select name="region" id="region">
                        <option value="Jizzax viloyati">Jizzax viloyati</option>
                        <option value="Namangan viloyati">Namangan viloyati</option>
                        <option value="Andijon viloyati">Andijon viloyati</option>
                        <option value="Farg'ona viloyati">Farg'ona viloyati</option>
                        <option value="Xorazm viloyati">Xorazm viloyati</option>
                        <option value="Navoyi viloyati">Navoyi viloyati</option>
                        <option value="Buxoro viloyati">Buxoro viloyati</option>
                        <option value="Qarshi viloyati">Qarshi viloyati</option>
                        <option value="Surxandaryo viloyati">Surxandaryo viloyati</option>
                        <option value="Sirdaryo viloyati">Sirdaryo viloyati</option>
                        <option value="Toshkent viloyati">Toshkent viloyati</option>
                        <option value="Qoraqalpogiston respublikasi">Qoraqalpogiston respublikasi</option>
                        <option value="Toshkent shahri">Toshkent shahri</option>

                    </select>
                </div>
                <div>
                    <p class="seleckt-name">Shahar/tuman</p>
                   <div class="select"> 
                       <select name="region" id="region">
                        <option value="denov">Do'stlik shahri</option>
                        <option value="denov">Yangiqo'rg'on tumani</option>
                        <option value="denov">Saraosiyo tumani</option>
                      </select>
                    </div>
                </div>
            </div>
            <div class="flex items-center gap-2 mt-5">
                <input type="checkbox" id="plant">
                <label for="plant">Mahallamga daraxt ekish</label>
            </div>
            <button class="btn gap-2 flex items-center mt-5">Davom etish
                <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M6.91075 15.5892C7.23618 15.9146 7.76382 15.9146 8.08926 15.5892L13.0893 10.5892C13.4147 10.2637 13.4147 9.7361 13.0893 9.41066L8.08926 4.41066C7.76382 4.08522 7.23618 4.08522 6.91075 4.41066C6.58531 4.7361 6.58531 5.26374 6.91075 5.58917L11.3215 9.99992L6.91075 14.4107C6.58531 14.7361 6.58531 15.2637 6.91075 15.5892Z" fill="white"/>
                </svg>

            </button>
        </div>
    </div>
       </div>
   </div>
</template>
<style scoped>
    .question{
        background: #46271A;
        color: #fff;
        padding: 46px 0 76px;
    }
    #region{
        outline: none;
        background: rgba(255, 255, 255, 0.1);
        border-radius: 8px;
        padding: 12px 16px;
    }
    .seleckt-name{
        font-weight: 400;
        font-size: 16px;
        line-height: 125%;
        opacity: 0.75;
        margin: 18px 0 6px;
    }
    .select-title{
        font-weight: 700;
        font-size: 24px;
        line-height: 30px;
    }
    .question-content{
        gap: 67px;
    }
    #plant{
        outline: none;
        background: rgba(255, 255, 255, 0.1);
    }
    input{
        background: rgba(255, 255, 255, 0.1);
    }
    .btn{
        background: rgba(255, 255, 255, 0.1);
        border-radius: 8px;
        padding: 12px 166px;
    }
    .img{
        width: 631px;
        height: 264px;
    }
    .select{
        background-color:  rgba(255, 255, 255, 0.1);
    }
</style>