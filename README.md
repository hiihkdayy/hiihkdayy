img/cloud.jpg
img/cloud1.png
img/loveHand.png
img/paperHeart.webp
img/squareLove.jpg
img/tickHeart.png
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./main.css">
    <!-- GOOGLE fONTS -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Protest+Riot&family=Rubik+Glitch+Pop&display=swap"
        rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Protest+Revolution&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&family=Pacifico&family=Protest+Revolution&display=swap" rel="stylesheet">
    <!--              -->
    <title>Valentine Day</title>
</head>

<body>
    <div class="container">
        <img class="paperHeart paperHeart1" style="--time: 0s" src="./img/paperHeart.webp" alt="">
        <img class="paperHeart paperHeart2" style="--time: 1s" src="./img/paperHeart.webp" alt="">
        <img class="paperHeart paperHeart3" style="--time: 2.5s" src="./img/paperHeart.webp" alt="">
        <img class="paperHeart paperHeart4" style="--time: 4s" src="./img/paperHeart.webp" alt="">
        <img class="paperHeart paperHeart5" style="--time: 2s" src="./img/paperHeart.webp" alt="">
        <img class="paperHeart paperHeart6" style="--time: 3s" src="./img/paperHeart.webp" alt="">

        <div class="boxTitle">
            <p class="firstTitle partTitle">Chúc mừng ngày mà pà</p>
            <p class="secondTitle partTitle"> đến với thế giới nàyy</p>
        </div>

        <div class="boxCloud">
            <div class="cloud"></div>
            <div class="cloud1"></div>
            <div class="cloud2"></div>

            <div class="btnBox">
                <div class="cloudBtn"></div>
                <button class="openBtn">Chạm vào đây đii bấy bii</button>
            </div>
        </div>

        <div class="cardValentine">
            <div class="left">
                <div class="leftFront">
                    <div class="boxShadow">
                        <div class="boxTitleCard"></div>
                    </div>

                    <p class="des">Hãy chạm vào tấm thiệp</p>
                </div>
                <div class="leftBack">
                    <img class="artHeart" src="./img/artHeart.webp" alt="">
                </div>
            </div>

            <div class="right">
                <div class="rightContent">
                    <p class="letterContent"></p>
                </div>
            </div>
        </div>
    </div>

    <script src="./main.js"></script>
</body>

</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    user-select: none;
}

html, body {
    height: 100%;
    width: 100%;
}

.container {
    position: relative;
    height: 100%;
    width: 100%;
    background-color: #fc6885;
    overflow: hidden;
}

.paperHeart {
    position: absolute;
    height: 100px;
    top: 80%;
    opacity: 0;
    filter: drop-shadow(0 0 20px rgb(247, 176, 176));
    animation: hiddenHeart 3.1s linear forwards,flyHeart 4s ease-in-out calc(var(--time) + 3.1s) infinite;
}

.paperHeart1 {
    left: 50px;
}

.paperHeart2 {
    left: 250px;
}

.paperHeart3 {
    left: 500px;
}

.paperHeart4 {
    left: 800px;
}

.paperHeart5 {
    left: 1100px;
}

.paperHeart6 {
    left: 1400px;
}

.boxCloud {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 300px;
    width: 100%;
    background-color: transparent;
}

.container .cloud {
    position: absolute;
    top: 120%;
    left: -50px;
}

.container .cloud1 {
    position: absolute;
    top: 120%;
    left: -50px;
}

.container .cloud2 {
    position: absolute;
    top: 120%;
    left: -50px;
}

.container.active.close {
    .btnBox {
        animation: disappearBtn 1s ease-in-out forwards;
    }

    .boxTitle {
        animation: disappearBoxTitle 1s ease-in-out forwards;
    }
}

@keyframes disappearBtn {
    from {
        top: 50%;
    }

    to {
        top: 150%;
    }
}

@keyframes disappearBoxTitle {
    from {
        top: 10%;
    }

    to {
        top: -50%;
    }
}

.container.active .cloud {
    position: absolute;
    top: 0;
    left: -50px;
    height: 200px;
    width: 200px;
    background-color: #ffb3c1;
    border-radius: 50%;
    box-shadow: 120px -20px #ffb3c1, 240px -40px #ffb3c1, 360px -20px #ffb3c1,
    480px 0px #ffb3c1, 600px -10px #ffb3c1, 720px 10px #ffb3c1, 840px 20px #ffb3c1, 
    960px 0px #ffb3c1, 1080px 40px #ffb3c1, 1200px 20px #ffb3c1, 1320px 0px #ffb3c1,
    1440px -20px #ffb3c1;
    transition: .8s;
    transition-delay: 2.2s;
    animation: animateCloud 3s ease-in-out 1s infinite;
}

@keyframes animateCloud {
    0% {
        top: 0;
    }

    25% {
        top:  10px;
    }

    50% {
        top: -10px;
    }

    75% {
        top: 10px;
    }

    100% {
        top: 0;
    }

}

@keyframes animateCloud1 {
    0% {
        top: 75;
    }

    25% {
        top:  85;
    }

    50% {
        top: 65;
    }

    75% {
        top: 85;
    }

    100% {
        top: 75;
    }

}

@keyframes animateCloud2 {
    0% {
        top: 150;
    }

    25% {
        top:  160px;
    }

    50% {
        top: 140px;
    }

    75% {
        top: 160px;
    }

    100% {
        top: 150;
    }

}

.container.active .cloud1 {
    position: absolute;
    top: 75px;
    left: -50px;
    content: "";
    height: 200px;
    width: 200px;
    background-color: #ffccd5;
    border-radius: 50%;
    box-shadow: 120px -20px #ffccd5, 240px -40px #ffccd5, 360px -20px #ffccd5,
    480px 0px #ffccd5, 600px -10px #ffccd5, 720px 10px #ffccd5, 840px 20px #ffccd5, 
    960px 0px #ffccd5, 1080px 40px #ffccd5, 1200px 20px #ffccd5, 1320px 0px #ffccd5,
    1440px -20px #ffccd5, 1560px 0px #ffccd5;
    transition: .8s;
    transition-delay: 1.3s;
    animation: animateClou1 3s ease-in-out 1.5s infinite;
}

.container.active .cloud2 {
    position: absolute;
    top: 150px;
    left: -50px;
    content: "";
    height: 200px;
    width: 200px;
    background-color: white;
    border-radius: 50%;
    box-shadow: 120px -20px white, 240px -20px white, 360px -20px white,
    480px 0px white, 600px -10px white, 720px 10px white, 840px 20px white, 
    960px 0px white, 1080px 40px white, 1200px 20px white, 1320px 0px white,
    1440px -20px white, 1560px 0px white;
    transition: .8s;
    transition-delay: .5s;
    animation: animateCloud2 3s ease-in-out 2s infinite;
}

.boxTitle {
    position: absolute;
    top: 120%;
    left: 50%;
    transform: translateX(-50%);
    font-family: "Rubik Glitch Pop", system-ui;
    font-weight: 400;
    font-style: normal;
    font-size: 120px;
    color: pink;
    height: fit-content;
    width: fit-content;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    text-shadow: 0 0 20px white;
    animation: appearTitle 2s linear 3.1s forwards, floatingWords 4s ease-in-out infinite;

}

.container .btnBox {
    position: absolute;
    top: 150%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 160px;
    width: 400px;
    opacity: 1;
}

.container.active .btnBox {
    opacity: 1;
    transition: 1s;
    transition-delay: 5s;
    animation: appearBtnBox 2s ease-in-out 5s forwards,animateOpenBtn 2s ease-in-out 5s infinite;
}

@keyframes appearBtnBox {
    from {
        top: 150%;
    }

    to {
        top: 50%;
    }
}

.cloudBtn {
    position: relative;
    height: 100px;
    width: 100px;
    background-color: #fc6885;
    border-radius: 50%;
    box-shadow: 60px 0 #fc6885, 120px 0 #fc6885, 180px 0 #fc6885, 240px 0 #fc6885,
    300px 0 #fc6885, 300px 60px #fc6885, 240px 60px #fc6885, 180px 60px #fc6885,
    120px 60px #fc6885, 60px 60px #fc6885, 0 60px #fc6885;
}

.cloudBtn::before {
    position: absolute;
    content: "";
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 80px;
    width: 80px;
    background-color: white;
    border-radius: 50%;
    box-shadow: 60px 0 white, 120px 0 white, 180px 0 white, 240px 0 white,
    300px 0 white, 300px 60px white, 240px 60px white, 180px 60px white,
    120px 60px white, 60px 60px white, 0 60px white;
}

.openBtn {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 100%;
    height: 100%;
    font-family: "Rubik Glitch Pop", system-ui;
    font-weight: 400;
    font-style: normal;
    font-size: 40px;
    color: #fc6885;
    background-color: transparent;
    border: none;
    text-shadow: 0 0 10px pink;
}

.openBtn:hover {
    cursor: grab;
}

/* OPEN */
.container.active.open {
    .boxTitle {
        animation: none;
        top: -40%;
    }

    .btnBox {
        animation: none;
        top: 140%;
    }

}

.cardValentine {
    position: absolute;
    top: 200%;
    left: 50%;
    opacity: 0;
    transform: translate(-50%, -50%);
    height: 600px;
    width: 800px;
    background-color: transparent;
    transition: .5;
}

.cardValentine.active {
    position: absolute;
    top: 50%;
    left: 50%;
    opacity: 1;
    transform: translate(-50%, -50%);
    height: 600px;
    width: 800px;
    background-color: transparent;
    transition: .5;
    animation: animateCard 2s ease-in-out forwards;
}

@keyframes animateCard {
    from {
        top: 200%;
    }

    to {
        top: 50%;
    }
}

.cardValentine .left {
    z-index: 2;
    position: absolute;
    top: 0;
    left: 50%;
    height: 100%;
    width: 50%;
    border-radius: 10px;
    transition: .5s;
    padding: 20px;
}

.cardValentine .left .leftFront {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background-color: #f35553;
    border-radius: inherit;
    transition: .5s;
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: 0 0 10px lightgray;
    border-left: 10px solid #c9413f;
}

.boxShadow {
    filter: drop-shadow(0 0 10px white);
    height: fit-content;
    width: fit-content;
}

.boxTitleCard {
    position: relative;
    height: 300px;
    width: 300px;
    display: flex;
    justify-content: center;
    background-color: white;
    clip-path: polygon(10% 0, 35% 0, 50% 23%, 65% 0, 90% 0, 100% 30%, 50% 100%, 0 30%);
}

.boxTitleCard::before {
    position: absolute;
    content: "";
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 280px;
    width: 280px;
    background-color: #f35553;
    clip-path: polygon(10% 0, 35% 0, 50% 23%, 65% 0, 90% 0, 100% 30%, 50% 100%, 0 30%);
}

.boxTitleCard::after {
    position: absolute;
    content: "";
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 250px;
    width: 250px;
    background-color: white;
    clip-path: polygon(10% 0, 35% 0, 50% 23%, 65% 0, 90% 0, 100% 30%, 50% 100%, 0 30%);
}


.titleCard {
    font-family: "Protest Revolution", sans-serif;
    font-weight: 400;
    font-style: normal;
    font-size: 60px;
    color: #f35553;
    margin-top: 80px;
}

.cardValentine .left .leftBack {
    position: absolute;
    top: 0;
    left: 0;
    transform: rotateY(180deg);
    backface-visibility: hidden;
    background-color: #f35553;
    height: 100%;
    width: 100%;
    border-radius: inherit;
    border-right: 10px solid #c9413f;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: .5s;
}

.artHeart {
    width: 90%;
    height: auto;
    filter: drop-shadow(0 0 5px white);
}

.des {
    position: absolute;
    bottom: 40px;
    left: 50%;
    transform: translateX(-50%);
    font-family: "Protest Revolution", sans-serif;
    font-weight: 400;
    font-size: 24px;
    font-style: normal;
    width: 100%;
    text-align: center;
}

.cardValentine .right {
    z-index: 1;
    position: absolute;
    top: 0;
    left: 50%;
    height: 100%;
    width: 50%;
    background-color: #f35553;
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-left: 10px solid #c9413f;
    transition: .5s;
}

.rightContent {
    font-size: 20px;
    height: 95%;
    width: 90%;
    background-color: wheat;
    border-radius: 5px;
    padding: 20px 15px;
    overflow: auto;
}

.rightContent::-webkit-scrollbar {
    background-color: white;
    width: 6px;
}

.rightContent::-webkit-scrollbar-thumb {
    background-color: #d34745;
}

.letterContent {
    font-family: "Pacifico", cursive;
    font-weight: 400;
    font-style: normal;
}

.cardValentine.active.open {
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    transition: .5s;

    .left {
        transform-style: preserve-3d;
        transform: rotateY(-180deg);
        transform-origin: left;
        background-color: red;
        transition: .5s;
    }

    .leftFront {
        backface-visibility: hidden;
    }

}

@keyframes appearTitle {
    to {
        top: 10%;
    }
}

@keyframes floatingWords {
    0% {
        transform: translateX(-50%);
    }

    25% {
        transform: translateX(-50%) translateY(-50px);
    }

    50% {
        transform: translateX(-50%) translateY(50px);
    }

    75% {
        transform: translateX(-50%) translateY(0);
    }
}

@keyframes flyHeart {
    to {
        top: -20%;
    }
}

@keyframes hiddenHeart {
    0% {
        opacity: 0;
    }

    95% {
        opacity: 0;
    }

    100% {
        opacity: 1;
    }
}

@keyframes animateOpenBtn {
    25% {
        top: 50%;
    }

    50% {
        top: calc(50% + 2px);
    }

    75% {
        top: calc(50% - 2px);
    }

    100% {
        top: 50%;
    }
}
var letterContent =" Chúc mừng sinh nhật pà nhee, ý là tui muốn làm cái này sớm hơn nhma lười quáa, chúc vịu ơ của hkim tủi 18 thật vuôi nhée, chúc dt sớm có 1 bờ vai vững chắc để dựa dẫm hen, hong được phép buồn bả trong tình cảm nữa, quên hết những chuyện buồn trong quá khứ đi nhé. Đặc biệt là tuôi gất là vuôi khi được chơi với pà á, dù là chỉ vỏn vẹn trong 3 năm cấp 3 thoii, nhma tuôi vẫn muốn được chơi với pà dài lâu á nhaa. Túm lại là CHÚC BÀ MỘT SINH NHẬT THẬT LÀ VUI VẺ VÀ HẠNH PHÚC NHÉ. LUV ❤️"

// Tốc độ viết chữ. Số càng nhỏ tốc độ càng nhanh. 50 là tốc độ khá phù hợp
durationWrite = 50 

// Hiệu ứng gõ chữ

function effectWrite () {
    var boxLetter = document.querySelector(".letterContent")
    letterContentSplited = letterContent.split("")

    letterContentSplited.forEach((val, index) => {
        setTimeout(() => {
            boxLetter.innerHTML += val    
        }, durationWrite* index)
    })
}

window.addEventListener("load", () => {
    setTimeout(() => {
        document.querySelector(".container").classList.add("active")
    }, 500)
})

var openBtn = document.querySelector(".openBtn")
openBtn.addEventListener("click", () => {
    document.querySelector(".cardValentine").classList.add("active")
    document.querySelector(".container").classList.add("close")
})

var cardValentine = document.querySelector(".cardValentine")

cardValentine.addEventListener("click", () => {
    cardValentine.classList.toggle("open")

    if(cardValentine.className.indexOf("open") != -1) {
        setTimeout(effectWrite, 500)
    } else {
        setTimeout(() => {
            document.querySelector(".letterContent").innerHTML = ""
        }, 1000)
    }
})
