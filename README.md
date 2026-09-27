<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>شمس ميثم — تسجيل الدخول</title>

<script src="https://unpkg.com/es-module-shims@1.7.0/dist/es-module-shims.js"></script>

<script type="importmap">
{
  "imports": {
    "@huggingface/hub": "https://cdn.jsdelivr.net/npm/@huggingface/hub@2.11.2/+esm"
  }
}
</script>

<style>

body{
    margin:0;
    min-height:100vh;

    display:flex;
    align-items:center;
    justify-content:center;

    font-family:
        Arial,
        "Segoe UI",
        sans-serif;

    background:
        linear-gradient(
            135deg,
            #fff0f7,
            #f0eaff
        );
}

.card{
    width:min(500px,90%);

    padding:40px;

    text-align:center;

    background:white;

    border-radius:28px;

    box-shadow:
        0 25px 70px
        rgba(100,50,100,.15);
}

.logo{
    width:70px;
    height:70px;

    margin:auto;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:22px;

    font-size:34px;

    color:white;

    background:
        linear-gradient(
            135deg,
            #e83f8f,
            #7956d8
        );
}

h1{
    margin:
        20px 0 8px;
}

p{
    color:#817681;
    line-height:1.7;
}

#signin{

    display:none;

    width:100%;

    margin-top:20px;

    padding:15px;

    border:0;

    border-radius:15px;

    background:
        #18141c;

    color:white;

    font-size:16px;

    font-weight:bold;

    cursor:pointer;
}

#signout{

    display:none;

    margin-top:20px;

    padding:12px 20px;

    border:0;

    border-radius:12px;

    background:#ffe7ee;

    color:#c33755;

    cursor:pointer;
}

#user{
    margin-top:20px;
    white-space:pre-wrap;
    direction:ltr;
    text-align:left;
    font-size:12px;
}

</style>

</head>


<body>


<div class="card">

    <div class="logo">
        ✨
    </div>

    <h1>
        شمس ميثم
    </h1>

    <p>
        تجميل وليزر
        <br>
        اختبار تسجيل الدخول بـ Hugging Face
    </p>


    <button id="signin">
        🤗 تسجيل الدخول بـ Hugging Face
    </button>


    <button id="signout">
        تسجيل الخروج
    </button>


    <pre id="user"></pre>

</div>



<script type="module">

import {
    oauthLoginUrl,
    oauthHandleRedirectIfPresent
}
from "@huggingface/hub";


/* =====================================
   عناصر الصفحة
===================================== */

const signin =
    document.getElementById("signin");

const signout =
    document.getElementById("signout");

const user =
    document.getElementById("user");


/* =====================================
   تسجيل الدخول
===================================== */

let oauthResult =
    localStorage.getItem("oauth");


/* استرجاع الجلسة */

if(oauthResult){

    try{

        oauthResult =
            JSON.parse(oauthResult);

    }catch{

        oauthResult =
            null;

    }

}


/* =====================================
   استقبال الرجوع من Hugging Face
===================================== */

oauthResult ||=
    await oauthHandleRedirectIfPresent();


/* =====================================
   إذا المستخدم مسجل
===================================== */

if(oauthResult){

    console.log(
        "OAuth result:",
        oauthResult
    );


    user.textContent =
        JSON.stringify(
            oauthResult,
            null,
            2
        );


    localStorage.setItem(
        "oauth",
        JSON.stringify(
            oauthResult
        )
    );


    signout.style.display =
        "inline-block";


    signin.style.display =
        "none";


    signout.onclick =
        function(){

            localStorage.removeItem(
                "oauth"
            );


            window.location.href =
                window.location.href
                .replace(/\?.*$/, '');

        };


}


/* =====================================
   إذا مو مسجل
===================================== */

else{

    signin.style.display =
        "block";


    signin.onclick =
        async function(){

            try{

                const url =
                    await oauthLoginUrl({

                        scopes:
                            window
                            .huggingface
                            .variables
                            .OAUTH_SCOPES

                    });


                /*
                 * نفتح OAuth خارج iframe
                 *
                 * هذا مهم حسب توثيق HF
                 */

                window.open(
                    url + "&prompt=consent",
                    "_blank"
                );


            }catch(error){

                console.error(
                    error
                );


                alert(
                    "خطأ في تسجيل الدخول:\n\n"
                    +
                    error.message
                );

            }

        };

}

</script>


</body>

</html>
