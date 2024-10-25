<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <script src="https://kit.fontawesome.com/19b3e5d630.js" crossorigin="anonymous"></script>
    <link rel="stylesheet" type="text/css" href="./style.css">
    <script src="https://unpkg.com/@dotlottie/player-component@latest/dist/dotlottie-player.mjs" type="module"></script>
    <title>Jecha Unemployed Time</title>
</head>

<body>
    <div class="clock-container">
        <div class="title">
            <h3>TODAY'S TIME TABLE </h1>
                <p>(NGANGGUR DAY)</p>
        </div>
        <br />

        <br />
        <div class="clock">
            <div class="clock-face">
                <div class="hour-mark" style="transform: rotate(0deg)">24</div>
                <div class="hour-mark" style="transform: rotate(15deg)">1</div>
                <div class="hour-mark" style="transform: rotate(30deg)">2</div>
                <div class="hour-mark" style="transform: rotate(45deg)">3</div>
                <link rel="stylesheet" type="text/css" href="./style.css">
                <div class="hour-mark" style="transform: rotate(60deg)">4</div>
                <div class="hour-mark" style="transform: rotate(75deg)">5</div>
                <div class="hour-mark" style="transform: rotate(90deg)">6</div>
                <div class="hour-mark" style="transform: rotate(105deg)">7</div>
                <div class="hour-mark" style="transform: rotate(120deg)">8</div>
                <div class="hour-mark" style="transform: rotate(135deg)">9</div>
                <div class="hour-mark" style="transform: rotate(150deg)">10</div>
                <div class="hour-mark" style="transform: rotate(165deg)">11</div>
                <div class="hour-mark" style="transform: rotate(180deg)">12</div>
                <div class="hour-mark" style="transform: rotate(195deg)">13</div>
                <div class="hour-mark" style="transform: rotate(210deg)">14</div>
                <div class="hour-mark" style="transform: rotate(225deg)">15</div>
                <div class="hour-mark" style="transform: rotate(240deg)">16</div>
                <div class="hour-mark" style="transform: rotate(255deg)">17</div>
                <div class="hour-mark" style="transform: rotate(270deg)">18</div>
                <div class="hour-mark" style="transform: rotate(285deg)">19</div>
                <div class="hour-mark" style="transform: rotate(300deg)">20</div>
                <div class="hour-mark" style="transform: rotate(315deg)">21</div>
                <div class="hour-mark" style="transform: rotate(330deg)">22</div>
                <div class="hour-mark" style="transform: rotate(345deg)">23</div>
            </div>

            <div class="divider" style="transform: rotate(330deg)"></div>
            <div class="divider" style="transform: rotate(75deg)"></div>
            <div class="divider" style="transform: rotate(90deg)"></div>
            <div class="divider" style="transform: rotate(135deg)"></div>
            <div class="divider" style="transform: rotate(165deg)"></div>
            <div class="divider" style="transform: rotate(180deg)"></div>
            <div class="divider" style="transform: rotate(225deg)"></div>
            <div class="divider" style="transform: rotate(270deg)"></div>
            <div class="divider" style="transform: rotate(300deg)"></div>
            <div class="divider" style="transform: rotate(315deg)"></div>

            <div class="label" style="--i: 23; --label-offset: -80px; --label-rotation: 15deg;">Sleep Time</div>
            <div class="label" style="--i: 5; --label-offset: -78px; --label-rotation: -75deg;">Morning</div>
            <div class="label" style="--i: 7.5; --label-offset: -70px; --label-rotation: -95deg;">Play Games</div>
            <div class="label" style="--i: 11.7; --label-offset: -73px; --label-rotation: -115deg;">Staying Blank</div>
            <div class="label" style="--i: 12.2; --label-offset: -100px; --label-rotation: -95deg;">Lunch</div>
            <div class="label" style="--i: 14.5; --label-offset: -105px; --label-rotation: 80deg;">Watch TV</div>
            <div class="label" style="--i: 17; --label-offset: -120px; --label-rotation: 90deg;">Take a nap</div>
            <div class="label" style="--i: 18.7; --label-offset: -125px; --label-rotation: 95deg;">Book Store</div>
            <div class="label" style="--i: 19.1; --label-offset: -125px; --label-rotation: 90deg;">Go to Comic</div>
            <div class="label" style="--i: 20.2; --label-offset: -130px; --label-rotation: 95deg;">Free Time</div>
            <div class="label" style="--i: 20.9; --label-offset: -125px; --label-rotation: 100deg;">Meditation</div>

            <link rel="stylesheet" type="text/css" href="./style.css">
            <div class="moon">
                <!-- <dotlottie-player src="https://lottie.host/bac9fd7f-fafd-4969-a137-09538eafdd43/y1TbRG8x9s.json"
                    background="transparent" speed="1" style="width: 120px; height: 120px;" loop
                    autoplay></dotlottie-player> -->

                <dotlottie-player src="https://lottie.host/0304c3e8-2fb8-4d73-99a1-32560919552e/6bJNTTJk7T.json"
                    background="transparent" speed="1" style="width: 120px; height: 100px;" loop
                    autoplay></dotlottie-player>
            </div>
            <div class="hand hour-hand"></div>
            <div class="hand minute-hand"></div>

            <div class="center" id="playButton">PLAY</div>
        </div>
        <br /><br />
        <div class="unit">
            Unit<br />
            DAY HOUR MINUTE
        </div>
    </div>
</body>
<script>
    function updateClock() {
        const now = new Date();
        const hours = now.getHours();
        const minutes = now.getMinutes();

        const hourDeg = (hours + minutes / 60) * 15;
        const minuteDeg = minutes * 6;

        document.querySelector(
            ".hour-hand"
        ).style.transform = `translateX(-50%) rotate(${hourDeg}deg)`;
        document.querySelector(
            ".minute-hand"
        ).style.transform = `translateX(-50%) rotate(${minuteDeg}deg)`;
    }

    setInterval(updateClock, 1000);
    updateClock();


</script>

<div id="player"></div>

<script src="https://www.youtube.com/iframe_api"></script>
<script>
    var player;
    function onYouTubeIframeAPIReady() {
        player = new YT.Player('player', {
            height: '0',
            width: '0',
            videoId: 'Av10eIyOF90',
            events: {
                'onReady': onPlayerReady
            }
        });
    }

    function onPlayerReady(event) {
        document.getElementById('playButton').addEventListener('click', function () {
            if (player.getPlayerState() == 1) {
                player.pauseVideo();
                this.textContent = 'PLAY';
            } else {
                player.playVideo();
                this.textContent = 'PAUSE';
            }
        });
    }
</script>

</html>