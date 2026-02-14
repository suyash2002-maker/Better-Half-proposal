<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instagram Proposal</title>

<style>
body{
    margin:0;
    background:#fafafa;
    font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}

/* Phone Frame */
.phone{
    width:380px;
    height:720px;
    background:white;
    border-radius:30px;
    box-shadow:0 10px 30px rgba(0,0,0,0.3);
    overflow:hidden;
    position:relative;
}

/* Top Bar */
.topbar{
    padding:12px;
    text-align:center;
    font-weight:bold;
    border-bottom:1px solid #ddd;
}

/* Header */
.header{
    display:flex;
    align-items:center;
    padding:10px;
}

.profile{
    width:35px;
    height:35px;
    border-radius:50%;
    background:linear-gradient(45deg,#feda75,#d62976,#962fbf);
    margin-right:10px;
}

.username{
    font-weight:bold;
}

/* Post Image */
.image{
    height:350px;
    background:linear-gradient(to bottom right,#ff4e50,#fc913a);
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    font-size:20px;
    padding:20px;
    cursor:pointer;
    position:relative;
}

/* Big Heart */
.big-heart{
    position:absolute;
    font-size:100px;
    color:white;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    opacity:0;
    transition:0.5s;
}

/* Actions */
.actions{
    padding:10px;
    font-size:24px;
}

.caption{
    padding:0 10px;
    font-size:14px;
}

.comments{
    padding:5px 10px;
    color:#555;
    font-size:13px;
}

/* Button */
button{
    background:#ff4e50;
    color:white;
    border:none;
    padding:10px 18px;
    border-radius:20px;
    margin:10px;
    cursor:pointer;
    font-size:14px;
}

/* Fireworks */
.firework{
    position:absolute;
    width:6px;
    height:6px;
    background:gold;
    border-radius:50%;
    animation:explode 1s ease-out forwards;
}

@keyframes explode{
    to{
        transform:translate(var(--x), var(--y));
        opacity:0;
    }
}
</style>
</head>

<body>

<div class="phone">
    <div class="topbar">Instagram</div>

    <div class="header">
        <div class="profile"></div>
        <div class="username">your_crush ❤️</div>
    </div>

    <div class="image" ondblclick="likePost()">
        💌 I’m Really Sorry 💌 <br><br>
        I never meant to hurt you...<br>
        You are my happiness 💕<br><br>
        Will you be my Valentine? 💘
        <div class="big-heart" id="bigHeart">❤️</div>
    </div>

    <div class="actions">
        ❤️ 💬 📤
    </div>

    <div class="caption">
        <b>you</b> One last chance to make it right 🥺💕
    </div>

    <div class="comments">
        best_friend: Say yes already 😍<br>
        mom: So cute ❤️
    </div>

    <button onclick="celebrate()">Say Yes 💖</button>

    <!-- Background Music -->
    <audio id="bgMusic" loop>
        <source src="romantic.mp3" type="audio/mp3">
    </audio>

</div>

<script>

/* Double Tap Like */
function likePost(){
    const heart = document.getElementById("bigHeart");
    heart.style.opacity = "1";
    setTimeout(()=>{ heart.style.opacity="0"; },800);
}

/* Celebrate + Music + Fireworks */
function celebrate(){
    let music = document.getElementById("bgMusic");

    // Fade-in Music
    music.volume = 0;
    music.play();
    let fade = setInterval(function(){
        if(music.volume < 1){
            music.volume += 0.05;
        } else {
            clearInterval(fade);
        }
    }, 200);

    // Fireworks
    for(let i=0;i<100;i++){
        const firework=document.createElement("div");
        firework.classList.add("firework");
        firework.style.left=Math.random()*380+"px";
        firework.style.top=Math.random()*600+"px";
        firework.style.setProperty('--x',(Math.random()*300-150)+'px');
        firework.style.setProperty('--y',(Math.random()*300-150)+'px');
        document.querySelector(".phone").appendChild(firework);
        setTimeout(()=>{firework.remove();},1000);
    }

    alert("She said YES! ❤️✨");
}

</script>

</body>
</html>
