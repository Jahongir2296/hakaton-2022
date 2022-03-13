<template>
    <div>
        <div class="my-9 ">
            <h1>Daraxt ekish</h1>
            <div class="flex gap-5">
                <div class="form-card p-6">
                    <div>
                      <div  class="flex gap-5">
                            <div class="left">
                            <label for="region">Viloyat</label><br>
                            <select name="region" id="region">
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                            </select>
                            <div class="checked flex gap-2 my-5">
                                <input class="w-6 h-6" type="checkbox">
                                <p>Mahallamga daraxt ekish</p>
                            </div>
                            <label for="destirict">Mahalla</label><br>
                            <select name="destirict" id="destirict">
                                <option value="Beruniy">Beruniy</option>
                                <option value="Bahor">Toshkent</option>
                                <option value="Tor">Beruniy</option>
                                <option value="Suyun">Beruniy</option>
                                <option value="Qora">Beruniy</option>

                            </select>
                        </div>
                          <div class="right">
                            <label for="city">Shahar</label><br>
                            <select name="city" id="city">
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                                <option value="Namangan">Namangan</option>
                            </select>
                        </div>
                      </div>
                      <div class="choice flex gap-5 items-end mt-5">
                          <div>
                              <label for="tree-type">Daraxt turi</label> <br>
                              <select name="tree-type" id="tree-type">
                                  <option value="manzarali">Manzarali</option>
                                  <option value="meva">Mevali daraxt</option>
                              </select>
                          </div>
                           <div>
                              <label for="tree-name">Daraxt nomi</label> <br>
                              <select name="tree-name" id="tree-name">
                                  <option value="manzarali">Archa</option>
                                  <option value="meva">Chinor</option>
                                  <option value="meva">Yapon noki</option> 
                              </select>
                          </div>
                          <div>
                              <label for="number">Soni</label> <br>
                              <input class="number-tree" type="number" placeholder="0">
                          </div>
                         <button>
                             <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd" d="M8 0C8.69762 0 9.26316 0.565535 9.26316 1.26316V6.73684H14.7368C15.4345 6.73684 16 7.30238 16 8C16 8.69762 15.4345 9.26316 14.7368 9.26316H9.26316V14.7368C9.26316 15.4345 8.69762 16 8 16C7.30238 16 6.73684 15.4345 6.73684 14.7368V9.26316H1.26316C0.565535 9.26316 0 8.69762 0 8C0 7.30238 0.565535 6.73684 1.26316 6.73684H6.73684V1.26316C6.73684 0.565535 7.30238 0 8 0Z" fill="white"/>
                            </svg>
                         </button>
                      </div>
                      <hr class="my-5 opacity-10">
                      <div class="relative">
                          <label for="social-link">Ijtimoiy tarmoqdagi sahifangiz uchun havolani kiriting:</label> <br>
                          <input id="social-link" type="text" class="relative" placeholder="https://">
                          <div class="social flex absolute gap-2">
                              <img class="w-5 h-5" src="../static/social/telegram.png" alt="">
                              <img class="w-5 h-5" src="../static/social/instagram.png" alt="">
                              <img class="w-5 h-5" src="../static/social/facebok.png" alt="">
                              <img class="w-5 h-5" src="../static/social/twitter.png" alt="">

                          </div>
                      </div>
                      <div class="flex mt-11 items-center">
                            <div class="flex gap-7 ">
                                <div class="flex gap-2">
                                    <input class="radio-pay" type="radio" name="pay" id="pay">
                                    <img class="pay-icon" src="../static/social/click.png" alt="">
                                </div>
                                  <div class="flex gap-2">
                                    <input class="radio-pay" type="radio" name="pay" id="pay">
                                    <img class="pay-icon" src="../static/social/payme.png" alt="">
                                </div>
                                  <div class="flex gap-2">
                                    <input class="radio-pay" type="radio" name="pay" id="pay">
                                    <img class="pay-icon" src="../static/social/apelsin.png" alt="">
                                </div>
                            </div>
                            <button class="send">
                                To'lovni amalga oshirish
                            </button>
                      </div>
                    </div>
                </div>
                <div class="overly">
                    <h2 class="overly-title">
                        Jami daraxtlar
                    </h2>
                    <hr>
                    <div class="mt-5  flex flex-col items-center gap-4">
                        <svg width="90" height="90" viewBox="0 0 90 90" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <g opacity="0.25" clip-path="url(#clip0_2_4773)">
                                <path d="M47.6365 53.1254V36.973C51.3807 36.7252 58.1106 35.6048 62.7541 30.9609C69.3555 24.3592 68.8385 13.5356 68.8134 13.0781C68.7394 11.7362 67.668 10.6646 66.3259 10.5906C65.8687 10.5652 55.045 10.0484 48.4435 16.6499C47.7411 17.3523 47.1201 18.1029 46.5697 18.8832C45.6026 14.9969 43.785 10.655 40.3876 7.25754C32.5023 -0.627696 19.5266 -0.00772535 18.9783 0.0228601C17.6364 0.0968627 16.5649 1.16841 16.4909 2.5103C16.4607 3.0589 15.8403 16.0347 23.7257 23.9201C29.5027 29.697 38.0103 30.9087 42.3631 31.1317V53.1254C43.2362 53.0274 44.1165 52.9767 44.9998 52.9767C45.8833 52.9767 46.7634 53.0275 47.6365 53.1254Z" fill="white"/>
                                <path d="M66.1808 68.8409C64.7628 68.8409 63.3664 69.0669 62.038 69.5055C60.8468 66.7236 58.9758 64.2415 56.595 62.3281C53.3231 59.6985 49.2052 58.2502 44.9998 58.2502C40.7947 58.2502 36.6767 59.6985 33.4046 62.3281C31.0239 64.2415 29.1529 66.7236 27.9617 69.5055C26.6333 69.0669 25.2368 68.8409 23.8189 68.8409C16.5255 68.8409 10.5918 74.7746 10.5918 82.0682V87.3635C10.5918 88.8196 11.7723 90.0002 13.2285 90.0002H76.771C78.2272 90.0002 79.4077 88.8196 79.4077 87.3635V82.0682C79.4079 74.7746 73.4743 68.8409 66.1808 68.8409Z" fill="white"/>
                            </g>
                            <defs>
                                <clipPath id="clip0_2_4773">
                                    <rect width="90" height="90" fill="white"/>
                                </clipPath>
                            </defs>
                        </svg>
                        <p>Daraxtlar tanlanmagan</p>

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .form-card{
        background: #1C2B27;
        border-radius: 16px;
    }
    select{
        background: rgba(255, 255, 255, 0.1);
        border: 1px solid rgba(255, 255, 255, 0.2);
        box-sizing: border-box;
        border-radius: 8px;
        padding: 12px 16px;
        outline: none;
    }
    label{
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        opacity: 0.75;
    }
    .number-tree{
        background: rgba(255, 255, 255, 0.1);
        border: 1px solid rgba(255, 255, 255, 0.2);
        box-sizing: border-box;
        border-radius: 8px;
        width: 101px;
        height: 50px;
        padding-left:10px ;
        outline: none;
    }
    .checkbox{
        width: 24px;
        height: 24px;
        margin-bottom: 20px;
    }
    button{
        background: rgba(255, 255, 255, 0.2);
        border-radius: 8px;
        width: 63px;
        height: 50px;
         padding-top: 3%;
        display: flex;
        justify-content: center;
    }
    .overly{
        background: #1C2B27;
        border-radius: 12px;
        padding: 24px;
        width: 384px;
        height: 262px;
    }
    .overly-title{
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 30px;
        padding-bottom: 14px;
    }
    #social-link{
        background: rgba(255, 255, 255, 0.1);
        border: 1px solid rgba(255, 255, 255, 0.2);
        box-sizing: border-box;
        border-radius: 8px;
        width: 740px;
        height: 44px;
        padding-left: 8px ;
        outline: none;
    }
    .social{
        background: rgba(255, 255, 255, 0.2);
        border-radius: 7px;
        width: 128px;
        height: 42px;
        right: 0;
        padding: 11px 12px;
        transform: translate(-1px, -43px);
    }
    .radio-pay{
        background: rgba(255, 255, 255, 0.1);
        border: 2px solid rgba(255, 255, 255, 0.2);
        box-sizing: border-box;
        border-radius: 8px;
        width: 20px;
        height: 20px;
    }
    .send{
        background: #5B6663;
        border-radius: 8px;
        width: 213px;
        height: 44px;
        font-weight: 700;
        font-size: 16px;
        line-height: 2px;
        color: #AEB4B2;
    }
    .pay-icon{
        height: 22px;
    }
</style>