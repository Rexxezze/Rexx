<!DOCTYPE html>
<html>
<head><meta name="viewport" content="width=device-width, initial-scale=1.0"></head>
  <title>My creation</title>
   
  <style>
    body {
      background: black;
      min-height: 100vh;
      color: white;
      text-align: center;
      font-family: Arial, Sans-Serif;
      overflow-x: hidden;
      
      box-shadow: inset 0 0 200px
    rgba(0,255,200,0.2);
    }

    h1 {
      opacity: 0;
      transform: translateY(50px);
      animation: masuk 1s ease forwards;
      font-size: 40px;
    }
    
    h2 {
     text-align: left;
     margin-left: 20px;
     margin-top: 200px;
   }

  .glitch {
  position: relative;
  font-size: 40px;
  color: white;
}
  .glitch::before,
  .glitch::after {
  content: attr(data-text);
  position: absolute;
  left: 0;
}
  .glitch::after {
  color: white;
  animation: glitch 0.3s infinite reverse;
}

  @keyframes glitch {
     0% { transform: translate(0); }
      20% { transform: translate(-2px, 2px); }
      40% { transform: translate(2px, -2px); }
     60% { transform: translate(-1px, 1px); }
     80% { transform: translate(1px, -1px); }
     100% { transform: translate(0); }
}

    @keyframes masuk {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    p {
      opacity: 0;
      transform: translateY(30px);
      animation: masuk 1s ease forwards;
      animation-delay: 0.5s;
      line-height: 1.5;
     font-size: 20px;
      color: #ccc;
      margin: 10px; 
      text-align: left;
    }
    
    p { 
      opacity: 0;
      transform: translateY(30px);
      animation: masuk 1s ease forwards;
      animation-delay: 0.5s;
      line-height: 1.5;
      font-size: 10px;
      color: #ccc;
      margin: 10px; 
      text-align: left;
    }

    .btn {
      margin-top: auto;
      padding: 12px 25px;
      background: white;
      color: black;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
      display: block;
      margin:auto;
      position: fixed;
      bottom: 200px;
      left:50% ;
      transform: translateX(-50%);
    }

    .btn:hover {
      transform: scale(1.1);
      background: gray;
    }

   .card {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%) scale(0);
  
      background: black;
      color: white;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 20px cyan;
      transition: 0.3s;
   }

.card.show {
  transform: translate(-50%, -50%) scale(1);
}


  </style>
</head>
 
<body>
  <h1>Hii</h1>
  <p>Discipline beats motivation. You might not feel like it, but if you keep going you still win. - David Goggins</p>
  <h2 class="glitch" data-text="HELLO">HELLO</h2>
  <p>Im Rexx, my real name is Iman. Im 14 years old, still a student, and a self-taught software engineer. I grew up spending a lot of time on computers, and now I enjoy building things using code. Im focused on improving my skills and learning new technologies.</p>
  <p>
I started coding when I was 11. At that time, I was bored of just playing Minecraft, Valorant, and trying to make games on Roblox. My daily routine felt repetitive, mostly chatting with friends and sitting all day. Then I discovered Discord bot templates and thought, what if I build one myself? That curiosity pushed me to start coding, and Ive been learning ever since.</p>
<button class="btn" onclick="buka()">Klik gua</button>

<div id="card" class="card">
  <h2>Thank you</h2>
  <p>Cuma test web btw</p>
</div>
</body>
<script>
function buka() {
  document.getElementById("card").classList.add("show");
}
</script>
</html>
