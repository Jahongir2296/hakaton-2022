<template>
    <div class="fresh ">
        <div class="container relative z-10">
            <h1 class="title">Har bir ekilgan daraxt kelajak uchun toza havoni taminlashga 
                yordam beradi! Hududingizni obodonlashtirishga befarq bolmang! 
            </h1>
            <p class="info mt-2">1ta daraxt 10 000 so'mdan</p>
            <button class="btn flex">Daraxt ekish 
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12.1569 8.81198C11.9312 8.90053 11.7097 8.6838 11.7845 8.45321C12.2982 6.87029 14.158 6.2798 15.8869 7.68416C16.7964 8.42296 17.1381 8.57994 17.1467 8.5839C16.5472 9.18333 15.8622 11.1948 14.3675 11.4173C12.7208 11.7158 11.2635 10.0958 12.4558 9.3545C13.24 8.86702 14.1632 8.58385 15.1528 8.58385C14.1153 8.34998 13.0796 8.45026 12.1569 8.81198Z" fill="#031410"/>
                    <path d="M4.70068 7.6842C7.68511 5.26001 9.58841 9.08299 8.40534 8.70403C7.56508 8.43488 6.64649 8.37626 5.72506 8.58394C7.28624 8.58394 8.72534 9.29939 9.68484 10.4639C9.60603 8.63384 9.48685 7.48829 9.34866 6.63615C8.55118 6.60874 7.4883 5.96476 6.90461 4.8379C5.89832 3.03702 6.36497 1.19053 6.51515 0.0253906C7.30144 0.791068 10.7362 -0.106104 12.0978 2.22717C12.6993 3.25787 12.5245 4.51211 11.8918 5.42994C11.6915 5.72051 11.2126 5.58109 11.1989 5.22847C11.1395 3.69455 10.376 2.53562 8.95284 1.89373C9.59146 2.72119 10.0108 3.64759 10.2274 4.6051C10.5641 6.09668 10.9158 7.07512 11.045 11.8292C11.0581 12.3113 10.6675 12.7104 10.1852 12.7044C9.83609 12.7 9.53701 12.4784 9.40274 12.1561C9.19853 11.6659 8.86615 11.1586 8.32529 10.6937C7.81131 11.2619 7.02919 11.5641 6.21993 11.4174C4.73152 11.1959 4.03689 9.18 3.44072 8.58389C3.44945 8.58003 3.79125 8.42305 4.70068 7.6842Z" fill="#031410"/>
                    <path d="M0.313532 13.6076C1.24652 12.9746 2.26196 13.4257 2.7283 13.6949L8.58045 17.9782L12.007 17.9789L12.8637 17.1223H9.71678C8.77035 17.1223 7.71042 16.5058 7.71042 15.4086C7.71042 14.2437 8.77035 13.6949 9.71678 13.6949H10.8961C11.7721 13.6949 12.7958 13.7731 13.5176 13.3867C14.2034 13.0377 14.9932 12.8391 15.8361 12.8391C17.2517 12.8391 18.5186 13.4034 19.3868 14.2934L24 18.8348L18.8601 23.9746L17.1469 21.4047H9.05074C8.1873 21.4047 7.35384 21.088 6.70836 20.5146L0.254959 14.7818C-0.103813 14.4631 -0.0835743 13.8771 0.313532 13.6076Z" fill="#031410"/>
                </svg>
            </button>
        </div>
    </div>
</template>

<style scoped>
    .fresh{
        position: relative;
        background-image: url(../static/fresh/bg-img.png);
        background-repeat: no-repeat;
        background-size: cover;
        padding: 83px 0 87px;
        color: #FFFFFF;
    }
    .fresh::after{
        content: "";
        position: absolute;
        background: linear-gradient(180deg, rgba(3, 20, 16, 0.4) 0%, #031410 100%);
        width: 100%;
        height: 452px;
        top: 0;
    }
    .title{
        font-weight: 700;
        font-size: 36px;
        line-height: 45px;
        max-width: 825px;
    }
    .info{
        font-weight: 400;
        font-size: 20px;
        line-height: 25px;
    }
    .btn{
        background: #FFFFFF;
        border-radius: 8px;
        font-weight: 700;
        font-size: 24px;
        line-height: 30px;
        color: #031410;
        padding: 16px 54px;
        margin-top: 53px;
    }
</style>