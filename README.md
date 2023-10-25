# Pokemon-collect-ball
body{
    background-image: url("assets/land.png");
}

.player{
    width: 80px;
    height: 100px;
    background-image: url("assets/player_front.png");
    background-size: 240px 100px;
    background-position: -80px 0;
    position: fixed;
    z-index: 999;
}
.player.active{
    animation: .2s walk linear infinite;
}

@keyframes walk{
    0%, 32%{
        background-position: 0 0;
    }
    33%, 65%{
        background-position: -80px 0;
    }
    66%, 100%{
        background-position: -160px 0;
    }
}

.bush{
    width: 50px;
    height: 40px;
    background-image: url("assets/bush.png");
    background-size: 100% 100%;
    position: fixed;
    z-index: -1;
}

.pokeball{
    width: 30px;
    height: 30px;
    background-image: url("assets/pokeball.png");
    background-size: 100% 100%;
    position: fixed;
}
