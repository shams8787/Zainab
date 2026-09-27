<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">

<meta
    name="viewport"
    content="width=device-width, initial-scale=1.0"
>

<title>
شمس ميثم | تجميل وليزر
</title>


<!-- PDF.JS -->

<script
    src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/4.10.38/pdf.min.mjs"
    type="module"
></script>


<style>

/* =========================================================
   SHAMS MAITHAM
   COSMETIC & LASER
========================================================= */

*{
    box-sizing:border-box;
}

:root{

    --pink:#e83f8f;

    --pink-light:#fff0f7;

    --pink-border:#f5c9df;

    --purple:#7956d8;

    --purple-light:#f0ebff;

    --dark:#29212b;

    --gray:#7c7180;

    --white:#ffffff;

    --background:#fff9fc;

    --green:#2eae76;

    --red:#df4662;

}


html{
    scroll-behavior:smooth;
}


body{

    margin:0;

    min-height:100vh;

    font-family:

        "Segoe UI",
        Tahoma,
        Arial,
        sans-serif;

    color:var(--dark);

    background:

        radial-gradient(
            circle at 90% 0%,
            #ffe1ef 0,
            transparent 28%
        ),

        radial-gradient(
            circle at 0% 90%,
            #e9e0ff 0,
            transparent 28%
        ),

        var(--background);

}


/* =========================================================
   HEADER
========================================================= */

.header{

    position:sticky;

    top:0;

    z-index:1000;

    display:flex;

    align-items:center;

    justify-content:space-between;

    gap:20px;

    padding:12px 22px;

    background:
        rgba(255,255,255,.88);

    backdrop-filter:
        blur(18px);

    border-bottom:
        1px solid var(--pink-border);

}


.brand{

    display:flex;

    align-items:center;

    gap:12px;

}


.logo{

    width:52px;

    height:52px;

    display:flex;

    align-items:center;

    justify-content:center;

    border-radius:18px;

    background:
        linear-gradient(
            135deg,
            var(--pink),
            var(--purple)
        );

    color:white;

    font-size:25px;

    box-shadow:
        0 8px 25px
        rgba(180,70,140,.22);

}


.brand-text h1{

    margin:0;

    font-size:18px;

}


.brand-text p{

    margin:2px 0 0;

    font-size:12px;

    color:var(--gray);

}


/* =========================================================
   LOGIN
========================================================= */

.login-button{

    border:0;

    padding:11px 17px;

    border-radius:13px;

    background:#18141c;

    color:white;

    font-weight:800;

    cursor:pointer;

    transition:.2s;

}


.login-button:hover{

    transform:
        translateY(-1px);

}


.user-box{

    display:none;

    align-items:center;

    gap:8px;

    padding:6px 8px;

    border-radius:15px;

    background:white;

    border:
        1px solid var(--pink-border);

}


.avatar{

    width:34px;

    height:34px;

    border-radius:50%;

    object-fit:cover;

}


.username{

    font-size:13px;

    font-weight:800;

}


.logout{

    border:0;

    background:#fff0f3;

    color:#c33452;

    padding:7px 10px;

    border-radius:9px;

    cursor:pointer;

}


/* =========================================================
   MAIN
========================================================= */

.container{

    width:
        min(1180px,94%);

    margin:auto;

}


/* =========================================================
   HERO
========================================================= */

.hero{

    padding:
        45px 0 25px;

}


.hero-card{

    position:relative;

    overflow:hidden;

    padding:42px;

    border-radius:30px;

    border:
        1px solid var(--pink-border);

    background:

        linear-gradient(
            135deg,
            rgba(255,255,255,.96),
            rgba(255,239,248,.95)
        );

    box-shadow:
        0 25px 70px
        rgba(100,50,100,.10);

}


.hero-card::after{

    content:"✦";

    position:absolute;

    left:-30px;

    bottom:-90px;

    font-size:230px;

    color:
        rgba(232,63,143,.05);

}


.badge{

    display:inline-flex;

    align-items:center;

    gap:5px;

    padding:
        7px 12px;

    border-radius:100px;

    background:#ffe5f1;

    color:#b72c6d;

    font-size:12px;

    font-weight:900;

}


.hero h2{

    max-width:800px;

    margin:
        17px 0 10px;

    font-size:
        clamp(32px,5vw,55px);

    line-height:1.08;

    background:

        linear-gradient(
            90deg,
            #d82e79,
            #7655d6
        );

    color:transparent;

    background-clip:text;

    -webkit-background-clip:text;

}


.hero-description{

    max-width:760px;

    color:var(--gray);

    line-height:1.9;

    margin:0;

}


/* =========================================================
   UPLOAD
========================================================= */

.upload{

    margin-top:25px;

    padding:35px 20px;

    border:
        2px dashed
        var(--pink-border);

    border-radius:23px;

    background:
        rgba(255,255,255,.7);

    text-align:center;

    cursor:pointer;

    transition:.2s;

}


.upload:hover{

    border-color:
        var(--pink);

    background:
        #fffafd;

}


.upload-icon{

    font-size:48px;

}


.upload h3{

    margin:
        8px 0 4px;

}


.upload p{

    margin:0;

    color:var(--gray);

    font-size:13px;

}


#pdf{

    display:none;

}


/* =========================================================
   BUTTONS
========================================================= */

.controls{

    display:flex;

    flex-wrap:wrap;

    gap:10px;

    margin-top:18px;

}


button{

    font-family:inherit;

}


.primary{

    border:0;

    padding:
        13px 20px;

    border-radius:14px;

    color:white;

    font-weight:900;

    cursor:pointer;

    background:

        linear-gradient(
            135deg,
            var(--pink),
            var(--purple)
        );

    box-shadow:
        0 10px 25px
        rgba(180,70,140,.18);

}


.secondary{

    border:
        1px solid var(--pink-border);

    padding:
        13px 20px;

    border-radius:14px;

    background:white;

    color:var(--dark);

    font-weight:800;

    cursor:pointer;

}


.stop{

    border:0;

    padding:
        13px 20px;

    border-radius:14px;

    background:#ffe8ed;

    color:#c03350;

    font-weight:900;

    cursor:pointer;

}


button:disabled{

    opacity:.45;

    cursor:not-allowed;

}


/* =========================================================
   STATUS
========================================================= */

.status{

    display:none;

    margin-top:22px;

    padding:18px;

    border:
        1px solid var(--pink-border);

    border-radius:18px;

    background:white;

}


.status-title{

    font-weight:900;

}


.status-text{

    margin-top:7px;

    font-size:13px;

    color:var(--gray);

}


.progress{

    height:11px;

    margin-top:13px;

    overflow:hidden;

    border-radius:100px;

    background:#f3e7ef;

}


.progress-bar{

    width:0%;

    height:100%;

    border-radius:100px;

    background:

        linear-gradient(
            90deg,
            var(--pink),
            var(--purple)
        );

    transition:.3s;

}


/* =========================================================
   SLIDES
========================================================= */

.slides{

    display:grid;

    gap:25px;

    margin:
        30px 0 60px;

}


.empty{

    padding:60px 20px;

    text-align:center;

    color:var(--gray);

}


.slide{

    overflow:hidden;

    border:
        1px solid var(--pink-border);

    border-radius:24px;

    background:white;

    box-shadow:
        0 12px 40px
        rgba(70,40,70,.06);

}


.slide-header{

    display:flex;

    justify-content:space-between;

    align-items:center;

    padding:
        15px 18px;

    background:
        #fffafd;

    border-bottom:
        1px solid var(--pink-border);

}


.slide-number{

    font-weight:950;

    color:#b72d6d;

}


.slide-state{

    padding:
        6px 10px;

    border-radius:100px;

    background:#f5eef5;

    color:var(--gray);

    font-size:11px;

    font-weight:800;

}


.slide-state.generating{

    background:#fff0d8;

    color:#9a6500;

}


.slide-state.done{

    background:#def8ec;

    color:#18835b;

}


.slide-content{

    padding:20px;

}


.two-columns{

    display:grid;

    grid-template-columns:
        1fr 1fr;

    gap:18px;

}


.panel{

    overflow:hidden;

    border:
        1px solid var(--pink-border);

    border-radius:17px;

    background:#fcfafd;

}


.panel-title{

    padding:
        11px 14px;

    background:white;

    border-bottom:
        1px solid var(--pink-border);

    font-size:13px;

    font-weight:900;

}


.panel-text{

    max-height:330px;

    overflow:auto;

    padding:14px;

    white-space:pre-wrap;

    line-height:1.75;

    font-size:13px;

    direction:auto;

}


.image-box{

    min-height:220px;

    display:flex;

    align-items:center;

    justify-content:center;

    margin-top:18px;

    overflow:hidden;

    border:
        1px solid var(--pink-border);

    border-radius:20px;

    background:#faf8fb;

}


.image-box img{

    width:100%;

    height:auto;

    display:block;

}


.placeholder{

    padding:40px;

    text-align:center;

    color:var(--gray);

}


.slide-buttons{

    display:flex;

    flex-wrap:wrap;

    gap:9px;

    margin-top:15px;

}


/* =========================================================
   FOOTER
========================================================= */

footer{

    padding:
        35px 20px;

    text-align:center;

    color:var(--gray);

    font-size:12px;

}


/* =========================================================
   MOBILE
========================================================= */

@media(max-width:760px){

    .header{

        padding:
            10px 12px;

    }


    .brand-text h1{

        font-size:15px;

    }


    .brand-text p{

        font-size:10px;

    }


    .hero-card{

        padding:
            25px 18px;

    }


    .two-columns{

        grid-template-columns:1fr;

    }


    .username{

        display:none;

    }


    .login-button{

        padding:
            9px 11px;

        font-size:11px;

    }

}

</style>

</head>


<body>


<!-- =====================================================
     HEADER
===================================================== -->

<header class="header">


    <div class="brand">

        <div class="logo">
            ✨
        </div>

        <div class="brand-text">

            <h1>
                شمس ميثم
            </h1>

            <p>
                تجميل وليزر
            </p>

        </div>

    </div>


    <div>

        <button
            id="loginButton"
            class="login-button"
        >
            🤗 تسجيل الدخول بـ Hugging Face
        </button>


        <div
            id="userBox"
            class="user-box"
        >

            <img
                id="avatar"
                class="avatar"
                src=""
                alt=""
            >

            <span
                id="username"
                class="username"
            >
            </span>

            <button
                id="logoutButton"
                class="logout"
            >
                خروج
            </button>

        </div>

    </div>


</header>


<!-- =====================================================
     MAIN
===================================================== -->

<main class="container">


<section class="hero">


<div class="hero-card">


    <span class="badge">
        ✨ SHAMS MAITHAM AI STUDY STUDIO
    </span>


    <h2>
        حوّلي محاضرتچ إلى
        صور تعليمية ✨
    </h2>


    <p class="hero-description">

        ارفعي محاضرة الـPDF،
        والموقع يقرأها من أول صفحة
        إلى آخر صفحة.
        لكل صفحة Prompt مستقل،
        وبعدها يتم توليد صورة تعليمية
        خاصة بيها.

    </p>


    <!-- UPLOAD -->

    <label
        for="pdf"
        class="upload"
    >

        <div class="upload-icon">
            📚
        </div>

        <h3>
            اختاري ملف المحاضرة
        </h3>

        <p>
            PDF فقط
        </p>

    </label>


    <input
        id="pdf"
        type="file"
        accept="application/pdf"
    >


    <!-- CONTROLS -->

    <div class="controls">


        <button
            id="readButton"
            class="primary"
            disabled
        >
            📖 قراءة المحاضرة
        </button>


        <button
            id="generateButton"
            class="primary"
            disabled
        >
            ✨ توليد كل الصور
        </button>


        <button
            id="stopButton"
            class="stop"
            disabled
        >
            ⏹ إيقاف
        </button>


        <button
            id="clearButton"
            class="secondary"
        >
            🗑️ مسح
        </button>


    </div>


    <!-- STATUS -->

    <div
        id="status"
        class="status"
    >

        <div
            id="statusTitle"
            class="status-title"
        >
            جاهز
        </div>


        <div
            id="progress"
            class="progress"
        >

            <div
                id="progressBar"
                class="progress-bar"
            >
            </div>

        </div>


        <div
            id="statusText"
            class="status-text"
        >
            -
        </div>

    </div>


</div>


</section>


<!-- =====================================================
     SLIDES
===================================================== -->

<section
    id="slides"
    class="slides"
>


    <div class="empty">

        📚

        <br><br>

        ارفعي محاضرة حتى تظهر السلايدات هنا

    </div>


</section>


</main>


<footer>

    ✨ شمس ميثم — تجميل وليزر

    <br><br>

    AI Educational Studio

</footer>



<!-- =====================================================
     APPLICATION
===================================================== -->

<script type="module">


/* =====================================================
   HUGGING FACE OAUTH
   OFFICIAL HF METHOD
===================================================== */

import {

    oauthLoginUrl,

    oauthHandleRedirectIfPresent

}

from
"https://cdn.jsdelivr.net/npm/@huggingface/hub/+esm";



let hfAuth = null;



/* =====================================================
   GET LOGIN BUTTON
===================================================== */

const loginButton =
    document.getElementById(
        "loginButton"
    );


const userBox =
    document.getElementById(
        "userBox"
    );


const username =
    document.getElementById(
        "username"
    );


const avatar =
    document.getElementById(
        "avatar"
    );


const logoutButton =
    document.getElementById(
        "logoutButton"
    );



/* =====================================================
   SHOW LOGGED USER
===================================================== */

function showLoggedUser(){

    if(!hfAuth)
        return;


    loginButton.style.display =
        "none";


    userBox.style.display =
        "flex";


    const user =
        hfAuth.userInfo;


    username.textContent =

        user?.preferred_username ||

        user?.name ||

        "Hugging Face";


    if(user?.picture){

        avatar.src =
            user.picture;

    }

}



/* =====================================================
   SHOW LOGOUT
===================================================== */

function showLoggedOut(){

    loginButton.style.display =
        "block";


    userBox.style.display =
        "none";

}



/* =====================================================
   INITIALIZE HF
===================================================== */

async function initializeHF(){

    try{


        /*
         * Hugging Face official function
         *
         * إذا رجعنا من OAuth:
         * ترجع معلومات المستخدم + token
         */

        const result =

            await oauthHandleRedirectIfPresent();


        if(result){

            hfAuth =
                result;


            /*
             * نخزن الجلسة مؤقتاً
             */

            sessionStorage.setItem(

                "shams_hf_auth",

                JSON.stringify(result)

            );


            showLoggedUser();


            console.log(
                "HF LOGIN:",
                result
            );


            return;

        }


        /*
         * إذا الصفحة انفتحت بدون callback
         * نحاول استعادة الجلسة
         */

        const saved =

            sessionStorage.getItem(
                "shams_hf_auth"
            );


        if(saved){

            try{

                hfAuth =
                    JSON.parse(saved);

                showLoggedUser();

                return;

            }catch(error){

                sessionStorage.removeItem(
                    "shams_hf_auth"
                );

            }

        }


        showLoggedOut();


    }catch(error){

        console.error(
            "HF OAuth initialization error:",
            error
        );


        showLoggedOut();

    }

}



/* =====================================================
   LOGIN
===================================================== */

loginButton.addEventListener(

    "click",

    async ()=>{

        try{


            /*
             * الرسمي في Static Space:
             *
             * لا نضع Client ID يدوياً.
             *
             * Hugging Face يقرأه من
             * Space config لأن README
             * يحتوي hf_oauth: true.
             */

            const url =

                await oauthLoginUrl();


            /*
             * فتح صفحة OAuth
             */

            window.location.href =
                url;


        }catch(error){

            console.error(
                "HF LOGIN ERROR:",
                error
            );


            alert(

                "ما قدر الموقع يفتح تسجيل الدخول.\n\n" +

                error.message

            );

        }

    }

);



/* =====================================================
   LOGOUT
===================================================== */

logoutButton.addEventListener(

    "click",

    ()=>{

        hfAuth =
            null;


        sessionStorage.removeItem(
            "shams_hf_auth"
        );


        location.reload();

    }

);



/* =====================================================
   START HF
===================================================== */

await initializeHF();



/* =====================================================
   PDF.JS
===================================================== */

const pdfjsLib =

    await import(

        "https://cdnjs.cloudflare.com/ajax/libs/pdf.js/4.10.38/pdf.min.mjs"

    );


pdfjsLib
.GlobalWorkerOptions
.workerSrc =

    "https://cdnjs.cloudflare.com/ajax/libs/pdf.js/4.10.38/pdf.worker.min.mjs";



/* =====================================================
   ELEMENTS
===================================================== */

const pdfInput =
    document.getElementById(
        "pdf"
    );


const readButton =
    document.getElementById(
        "readButton"
    );


const generateButton =
    document.getElementById(
        "generateButton"
    );


const stopButton =
    document.getElementById(
        "stopButton"
    );


const clearButton =
    document.getElementById(
        "clearButton"
    );


const slidesElement =
    document.getElementById(
        "slides"
    );


const status =
    document.getElementById(
        "status"
    );


const statusTitle =
    document.getElementById(
        "statusTitle"
    );


const statusText =
    document.getElementById(
        "statusText"
    );


const progressBar =
    document.getElementById(
        "progressBar"
    );



/* =====================================================
   VARIABLES
===================================================== */

let selectedPDF =
    null;


let slides =
    [];


let stopRequested =
    false;



/* =====================================================
   FIXED PROMPT
===================================================== */

const FIXED_PROMPT =

"Make a diagram showing the following write and draw every detail (dont skip any word & dont add any word) use alot of drawings & illustrations (white background)";



/* =====================================================
   SELECT PDF
===================================================== */

pdfInput.addEventListener(

    "change",

    ()=>{

        selectedPDF =
            pdfInput.files[0];


        if(!selectedPDF)
            return;


        readButton.disabled =
            false;


        generateButton.disabled =
            true;


        slides = [];


        slidesElement.innerHTML =

            `<div class="empty">
                📄 تم اختيار:
                <br><br>
                <b>${escapeHTML(selectedPDF.name)}</b>
                <br><br>
                اضغطي "قراءة المحاضرة"
            </div>`;


        setStatus(

            "تم اختيار الملف",

            selectedPDF.name,

            0

        );

    }

);



/* =====================================================
   READ PDF
===================================================== */

readButton.addEventListener(

    "click",

    async ()=>{

        if(!selectedPDF)
            return;


        readButton.disabled =
            true;


        generateButton.disabled =
            true;


        slides = [];


        try{


            setStatus(

                "جاري قراءة المحاضرة",

                "يتم استخراج كل الصفحات...",

                0

            );


            const buffer =

                await selectedPDF.arrayBuffer();


            const pdf =

                await pdfjsLib
                .getDocument({
                    data:buffer
                })
                .promise;


            const total =
                pdf.numPages;


            /*
             * نقرأ كل صفحة
             */

            for(

                let pageNumber = 1;

                pageNumber <= total;

                pageNumber++

            ){


                const page =

                    await pdf.getPage(
                        pageNumber
                    );


                const content =

                    await page
                    .getTextContent();


                /*
                 * النص الأصلي
                 */

                const originalText =

                    content.items

                    .map(
                        item =>
                            item.str
                    )

                    .join(" ")

                    .trim();


                /*
                 * Prompt خاص بالسلايد
                 */

                const prompt =

                    originalText +

                    "\n\n" +

                    FIXED_PROMPT;


                slides.push({

                    number:
                        pageNumber,

                    text:
                        originalText,

                    prompt:
                        prompt,

                    image:
                        null,

                    state:
                        "waiting"

                });


                updateProgress(

                    pageNumber,

                    total,

                    `قراءة الصفحة ${pageNumber} من ${total}`

                );

            }


            renderSlides();


            generateButton.disabled =
                slides.length === 0;


            setStatus(

                "تمت القراءة ✨",

                `تم العثور على ${slides.length} صفحة. لا توجد عملية اختصار.`,

                100

            );


        }catch(error){

            console.error(error);


            setStatus(

                "حدث خطأ",

                error.message,

                0

            );

        }finally{

            readButton.disabled =
                false;

        }

    }

);



/* =====================================================
   RENDER ALL SLIDES
===================================================== */

function renderSlides(){

    slidesElement.innerHTML = "";


    if(!slides.length){

        slidesElement.innerHTML =

            `<div class="empty">
                لا توجد صفحات
            </div>`;

        return;

    }


    slides.forEach(

        slide=>{


            const article =

                document.createElement(
                    "article"
                );


            article.className =
                "slide";


            article.id =
                `slide-${slide.number}`;


            article.innerHTML = `

                <div class="slide-header">

                    <div class="slide-number">

                        📄 الصفحة
                        ${slide.number}

                    </div>

                    <div
                        id="state-${slide.number}"
                        class="slide-state"
                    >

                        بانتظار التوليد

                    </div>

                </div>


                <div class="slide-content">


                    <div class="two-columns">


                        <div class="panel">

                            <div class="panel-title">

                                📖 النص الأصلي

                            </div>

                            <div class="panel-text">

                                ${escapeHTML(slide.text)}

                            </div>

                        </div>


                        <div class="panel">

                            <div class="panel-title">

                                ✨ Prompt هذا السلايد

                            </div>

                            <div class="panel-text">

                                ${escapeHTML(slide.prompt)}

                            </div>

                        </div>


                    </div>


                    <div
                        id="image-${slide.number}"
                        class="image-box"
                    >

                        <div class="placeholder">

                            🖼️

                            <br><br>

                            لم يتم توليد الصورة بعد

                        </div>

                    </div>


                    <div class="slide-buttons">


                        <button
                            class="primary"
                            data-slide="${slide.number}"
                        >

                            ✨ توليد هذا السلايد

                        </button>


                    </div>


                </div>

            `;


            slidesElement.appendChild(
                article
            );


            const button =

                article.querySelector(
                    "button"
                );


            button.addEventListener(

                "click",

                ()=>{

                    generateSingleSlide(
                        slide.number
                    );

                }

            );

        }

    );

}



/* =====================================================
   GENERATE ALL
===================================================== */

generateButton.addEventListener(

    "click",

    async ()=>{


        /*
         * لازم المستخدم يكون داخل
         */

        if(!hfAuth){

            alert(
                "سجلي دخول Hugging Face أولاً."
            );

            return;

        }


        if(!slides.length)
            return;


        stopRequested =
            false;


        stopButton.disabled =
            false;


        generateButton.disabled =
            true;


        /*
         * نبدأ من أول سلايد
         *
         * إذا كان عنده صورة
         * نتخطاه.
         */

        for(

            let i = 0;

            i < slides.length;

            i++

        ){


            if(stopRequested)
                break;


            const slide =
                slides[i];


            /*
             * استكمال
             */

            if(slide.image)
                continue;


            await generateSlide(
                slide
            );


            updateProgress(

                i + 1,

                slides.length,

                `توليد الصفحة ${i+1} من ${slides.length}`

            );

        }


        stopButton.disabled =
            true;


        generateButton.disabled =
            false;


        if(stopRequested){

            setStatus(

                "تم الإيقاف ⏹",

                "تقدرين تضغطين توليد مرة ثانية حتى يكمل من حيث توقف.",

                getCompletedPercent()

            );

        }else{

            setStatus(

                "اكتملت المحاضرة ✨",

                `تمت معالجة ${slides.length} صفحة.`,

                100

            );

        }

    }

);



/* =====================================================
   STOP
===================================================== */

stopButton.addEventListener(

    "click",

    ()=>{

        stopRequested =
            true;


        stopButton.disabled =
            true;

    }

);



/* =====================================================
   GENERATE SINGLE
===================================================== */

async function generateSingleSlide(
    number
){

    if(!hfAuth){

        alert(
            "سجلي دخول Hugging Face أولاً."
        );

        return;

    }


    const slide =

        slides.find(
            s =>
                s.number === number
        );


    if(!slide)
        return;


    await generateSlide(
        slide
    );

}



/* =====================================================
   GENERATE IMAGE
===================================================== */

async function generateSlide(
    slide
){

    setSlideState(

        slide.number,

        "generating",

        "جاري التوليد..."

    );


    try{


        /*
         * Access token من OAuth
         */

        const token =
            hfAuth.accessToken;


        if(!token){

            throw new Error(
                "لم يتم الحصول على Hugging Face access token."
            );

        }


        /*
         * Hugging Face Inference Router
         */

        const response =

            await fetch(

                "https://router.huggingface.co/hf-inference/models/black-forest-labs/FLUX.1-schnell",

                {

                    method:"POST",

                    headers:{

                        "Authorization":
                            `Bearer ${token}`,

                        "Content-Type":
                            "application/json"

                    },

                    body:
                        JSON.stringify({

                            inputs:
                                slide.prompt

                        })

                }

            );


        if(!response.ok){

            const errorText =
                await response.text();


            throw new Error(

                `Hugging Face ${response.status}: ${errorText}`

            );

        }


        const blob =
            await response.blob();


        const imageURL =
            URL.createObjectURL(
                blob
            );


        slide.image =
            imageURL;


        slide.state =
            "done";


        showImage(

            slide.number,

            imageURL

        );


        setSlideState(

            slide.number,

            "done",

            "تم التوليد ✓"

        );


    }catch(error){

        console.error(
            error
        );


        setSlideState(

            slide.number,

            "",

            "فشل التوليد"

        );


        const imageBox =

            document.getElementById(

                `image-${slide.number}`

            );


        imageBox.innerHTML = `

            <div class="placeholder">

                ❌

                <br><br>

                ${escapeHTML(error.message)}

            </div>

        `;

    }

}



/* =====================================================
   SHOW IMAGE
===================================================== */

function showImage(

    number,

    url

){

    const box =

        document.getElementById(

            `image-${number}`

        );


    box.innerHTML = "";


    const image =
        document.createElement(
            "img"
        );


    image.src =
        url;


    image.alt =
        `Shams Maitham educational slide ${number}`;


    box.appendChild(
        image
    );

}



/* =====================================================
   SLIDE STATE
===================================================== */

function setSlideState(

    number,

    type,

    text

){

    const state =

        document.getElementById(

            `state-${number}`

        );


    if(!state)
        return;


    state.textContent =
        text;


    state.className =
        "slide-state " +
        (
            type || ""
        );

}



/* =====================================================
   STATUS
===================================================== */

function setStatus(

    title,

    text,

    percent

){

    status.style.display =
        "block";


    statusTitle.textContent =
        title;


    statusText.textContent =
        text;


    progressBar.style.width =
        `${percent}%`;

}



/* =====================================================
   PROGRESS
===================================================== */

function updateProgress(

    current,

    total,

    text

){

    const percent =

        Math.round(

            current /
            total *
            100

        );


    setStatus(

        `${percent}%`,

        text,

        percent

    );

}



/* =====================================================
   COMPLETED %
===================================================== */

function getCompletedPercent(){

    if(!slides.length)
        return 0;


    const completed =

        slides.filter(
            slide =>
                slide.image
        ).length;


    return Math.round(

        completed /
        slides.length *
        100

    );

}



/* =====================================================
   CLEAR
===================================================== */

clearButton.addEventListener(

    "click",

    ()=>{

        selectedPDF =
            null;


        slides =
            [];


        pdfInput.value =
            "";


        readButton.disabled =
            true;


        generateButton.disabled =
            true;


        stopButton.disabled =
            true;


        slidesElement.innerHTML =

            `<div class="empty">

                📚

                <br><br>

                ارفعي محاضرة حتى تظهر السلايدات هنا

            </div>`;


        status.style.display =
            "none";


        progressBar.style.width =
            "0%";

    }

);



/* =====================================================
   ESCAPE HTML
===================================================== */

function escapeHTML(
    value
){

    return String(value)

        .replaceAll(
            "&",
            "&amp;"
        )

        .replaceAll(
            "<",
            "&lt;"
        )

        .replaceAll(
            ">",
            "&gt;"
        )

        .replaceAll(
            '"',
            "&quot;"
        )

        .replaceAll(
            "'",
            "&#039;"
        );

}

</script>


</body>

</html>
