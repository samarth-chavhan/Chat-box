# Chat-box
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Google (Kids mode)</title>
        <link rel="icon" href="Google logo.png" type="image/x-icon" />
        <style>    @import url('https://fonts.googleapis.com/css2?family=Mukta:wght@200;300;400;500;600;700;800&display=swap');
    body {
        margin: 0;
        padding: 0;
        background-color: #212121;
        font-family: Arial,sans-serif; 
    }
    .gap {
        height: 16rem;
    }
    #logo {
        height: 6em;
        margin-bottom: .5rem;
    }
    main {
        display: flex;
        justify-content: center;
    }
    .search-bar {
        display: flex;
        justify-content: center;    
        align-items: center;
        flex-direction: column;
    }
    #search{
        border-radius: 1.2rem;
        width:30rem;
        height: 2.5rem;
        border: .3px solid white;
        background-color: #1c1c1b;
        margin-bottom: 1.5rem;
        margin-top: 0.5rem;
        color:white;
        font-size: 1rem;
        padding-left: 2rem;
    }
    #search:focus{
        outline:none
    }
    #Google{
        color:white;
        display: flex;
        justify-content: center;
        text-align: center;
    }
    footer{
        margin-top:1rem;
    }
    a{
        color:lightblue;
        text-decoration: none;
    }
    a:hover{
        text-decoration:underline
    }
    button{
        background-color: #303134;
        border: 1px solid #303134;
        border-radius: 4px;
        color: #e8eaed;
        font-family: arial, sans-serif;
        font-size: 14px;
        margin: 11px 4px;
        padding: 0 16px;
        line-height: 27px;
        height: 36px;
        min-width: 54px;
        text-align: center;
        cursor: pointer;
        user-select: none;
    }
    button:hover{
        text-decoration: none;
    }
    @keyframes vibrate {
        0% { transform: translateX(-1px); }
        25% { transform: translateX(1px); }
        50% { transform: translateX(-1px); }
        75% { transform: translateX(1px); }
        100% { transform: translateX(0); } /* Return to original position */
    }
    
    .vibrate {
        animation: vibrate 0.1s infinite;
    }
    </style>
    </head>
    <body>
        <div class="gap"></div>
        <main>
            <div>
                <img src="logo.png" alt="Google logo" id="logo" />
            </div>  
        </main>
        <section class="search-bar">
                <div>
                <div id="div"></div>
                <input type="search"  id="search" oninput="saveSearch()" />
            </div>
            <div>
                <a href="#" id="link" onkeydown="if(event.key==='Enter') { search(); return false; }">
                    <button onclick="search()">Google search</button>
                    <a href="https://doodles.google/">
                        <button>I'm Feeling Lucky</button>
                    </a>    
            </div>
        </section>
        <footer>
            <div id="Google">Google offered in:
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=hi&source=homepage&sa=X&ved=0ahUKEwjxyYin_P2FAxUY2TQHHc_pB4wQ2ZgBCCE">हिन्दी</a> &nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=bn&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCI">বাংলা</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=te&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCM">తెలుగు</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=mr&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCQ">मराठी</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=ta&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCU">தமிழ்</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=gu&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCY">ગુજરાતી</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=kn&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCc">ಕನ್ನಡ</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=ml&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCg">മലയാളം</a>&nbsp;&nbsp;&nbsp;
            <a href="https://www.google.com/setprefs?sig=0_v9RIJqE-cfZYQswYR5pG3gr5NN0%3D&hl=pa&source=homepage&sa=X&ved=0ahUKEwiGhIebg_6FAxWV2DQHHZmRC_MQ2ZgBCCk">ਪੰਜਾਬੀ</a>&nbsp;&nbsp;&nbsp;

        </footer>
        <script>function search() {
    let search = document.getElementById("search").value;
    let link = document.getElementById("link");
    link.href = `https://google.com/search?q= ${search}`
    link.target = _blank;
}
let border = document.getElementById("search")

function saveSearch() {
    let searchValue = document.getElementById("search").value.toLowerCase();
    localStorage.setItem("searchInput", searchValue);
    switch (searchValue) {
        case "xxx":
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "xxx videos" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "xhamster":
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "pornhub" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "sex":
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "nudes" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "nudes" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "porn" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
        case "18+" :
            border.style.border = "1px solid red";
            border.classList.add("vibrate");
            setTimeout(() => {
                border.classList.remove("vibrate");
                alerts()
            }, Infinity);
            function alerts() {
                alert("Don't Search This Things")
            }
            break;
    
        default:
            border.style.border = "0.3px solid white"; 
        border.classList.remove("vibrate");
            break;
    }
}
</script>
    </body>
    </html>

