<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Quà 19/11</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');
body{
  margin:0;
  font-family:'Poppins',sans-serif;
  background:linear-gradient(135deg,#ff6ec7,#ff9acb,#ffd1e8,#ffe6f3);
  background-size:400% 400%;
  animation:bgflow 10s ease infinite;
  color:#fff;
  overflow-x:hidden;
}
@keyframes bgflow{0%{background-position:0% 50%;}50%{background-position:100% 50%;}100%{background-position:0% 50%;}}
.page{
  display:none;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  min-height:100vh;
  padding:20px;
  text-align:center;
  animation:fade .8s ease;
}
@keyframes fade{from{opacity:0;transform:translateY(20px);} to{opacity:1;transform:translateY(0);}}
button{
  padding:12px 30px;
  font-size:20px;
  border:none;
  border-radius:18px;
  background:linear-gradient(135deg,#ff4f93,#ff74b8);
  color:#fff;
  box-shadow:0 5px 20px rgba(0,0,0,0.25);
  cursor:pointer;
  margin:10px 0;
  transition:0.3s;
}
button:hover{transform:scale(1.07); box-shadow:0 8px 25px rgba(0,0,0,0.3);}
img.correct{max-width:90%; height:auto; border-radius:20px; box-shadow:0 12px 35px rgba(255,105,180,0.6); animation:pop .6s ease; margin:15px 0;}
img.wrong{max-width:70%; height:auto; border-radius:20px; opacity:0.8; box-shadow:0 5px 15px rgba(0,0,0,0.25); animation:shake 0.5s; margin:15px 0;}
@keyframes pop{from{transform:scale(0.7);opacity:0;} to{transform:scale(1);opacity:1;}}
@keyframes shake{0%{transform:translateX(0);}25%{transform:translateX(-10px);}50%{transform:translateX(10px);}75%{transform:translateX(-10px);}100%{transform:translateX(0);}}
#pinkboard{width:100%; height:100%; display:block;}
</style>
</head>
<body>

<!-- PAGE 1 -->
<div id="p1" class="page" style="display:flex;">
  <h1 style="font-size:40px; text-shadow:0 4px 20px rgba(255,0,140,0.5);">✨ Quà 19/11 dành cho anh ✨</h1>
  <button onclick="go('q1')">Click vô đây nè 💗</button>
</div>

<!-- QUESTION 1 -->
<div id="q1" class="page">
  <h2 style="font-size:32px;">Câu 1: Gọi em bằng gì? 😏</h2>
  <button onclick="checkQ1('A')">A: mày</button>
  <button onclick="checkQ1('B')">B: Con nhỏ này</button>
  <button onclick="checkQ1('C')">C: Bằng mồm 😳</button>
  <button onclick="checkQ1('D')">D: Em gái 💗</button>
</div>
<div id="q1_correct" class="page">
  <h2>Đúm òi nè chiều ông ơiiiii,chọn đáp án gọi bằng mồm thì mình phải sao ạaaaaaaaa😚💗</h2>
  <img src="https://i.ibb.co/pvSJwM03/retouch-2025062418044691.jpg" class="correct" />
</div>
<div id="q1_wrong" class="page">
  <h2>Ôi sai rồi 😤</h2>
  <img src="https://i.ibb.co/zV1N6ptt/225424-thuoc-la-sai-gon-peach.webp" class="wrong" />
  <button onclick="go('q1')">Chọn lại 😒</button>
</div>

<!-- QUESTION 2 -->
<div id="q2" class="page">
  <h2 style="font-size:32px;">Câu 2: Nay ngày gì vậy hmmm? 🎀</h2>
  <button onclick="checkQ2('A')">A: Ngày em đến 💗</button>
  <button onclick="checkQ2('B')">B: Ngày anh có quà 🎁</button>
  <button onclick="checkQ2('C')">C: 19/11 ✨</button>
  <button onclick="checkQ2('D')">D: BC 🤨</button>
</div>
<div id="q2_correct" class="page">
  <h2>Giỏi quá taaaaaa 😚💗</h2>
  <img src="https://i.ibb.co/dwfGWknb/retouch-2025100119330187.jpg" class="correct" />
  <button id="heartBtn">Bấm trái tim 💓</button>
</div>
<div id="q2_wrong" class="page">
  <h2>Trời ơi… chọn lại lẹ 😤</h2>
  <img src="https://i.ibb.co/zV1N6ptt/225424-thuoc-la-sai-gon-peach.webp" class="wrong" />
  <button onclick="go('q2')">Chọn lại 😒</button>
</div>

<!-- HEART EFFECT PAGE -->
<div id="heartEffect" class="page">
  <div style="position:relative; width:100%; height:70vh;">
    <canvas id="pinkboard"></canvas>
  </div>
  <button onclick="go('gift')">Next / Bỏ qua</button>
</div>

<!-- GIFT PAGE -->
<div id="gift" class="page" style="flex-direction:column; align-items:center;">
  <div id="letterWrapper" style="perspective:1000px; width:90%; max-width:600px; margin-bottom:25px;">
    <div id="letter" style="
        background:#fff4e6; color:#5a3e36; padding:30px 25px; border:2px solid #d8b88b; 
        border-radius:15px; box-shadow:0 10px 30px rgba(0,0,0,0.2); font-family:'Cursive','Poppins',sans-serif; 
        text-align:left; line-height:1.6; transform: rotateX(-90deg); transform-origin:top; transition: transform 1.5s ease;">
      <h2 style="text-align:center; font-family:'Poppins',sans-serif; color:#ff4f93;">💌TÂM SỰ NHỎ TỪ MÁ NHỎ</h2>
      <p>Sói của em ơiiiiiiii!,</p>
      <p>Hôm nay là ngày đặc biệt,với cái tâm thế ngày này không thể để boy của em thiệt thòi.Em muốn gửi đến anh món quà nhỏ này kèm theo lời chúc từ tận trái tim em.</p>
      <p>Chúc anh luôn vui vẻ, mạnh khỏe, hạnh phúc và mọi điều tốt đẹp đều đến với anh 💖✨</p>
      <p>Mong rằng món quà này sẽ làm anh cười và nhớ đến em mỗi khi nhìn thấy ạaaaaaa 💗</p>
      <p>Yêu anh nhiều lắm ạaaaaaaa,<br>Mthuw 💌</p>
    </div>
  </div>
  <div id="finalGift" style="opacity:0; text-align:center; transition:opacity 1s ease;">
    <h2 style="font-size:24px; color:#ff4f93; margin-bottom:15px; text-shadow:0 2px 8px rgba(0,0,0,0.3);">
      💖 Bây giờ hãy mở món quà ra đi nèeee 💖
    </h2>
    <img id="giftImg" src="https://i.ibb.co/fYbRGYV8/Video-Capture-20250817-182200.jpg" 
         style="max-width:80%; height:auto; border-radius:15px; box-shadow:0 10px 25px rgba(0,0,0,0.25);" />
  </div>
</div>

<script>
// Chuyển trang
function go(id){
  document.querySelectorAll('.page').forEach(p=>p.style.display='none');
  const page = document.getElementById(id);
  page.style.display='flex';
  if(id==='gift') openLetterFold();
}

// Câu hỏi
function checkQ1(a){ a==='C'? (go('q1_correct'), setTimeout(()=>go('q2'),1500)) : go('q1_wrong'); }
function checkQ2(a){ a==='D'? go('q2_correct') : go('q2_wrong'); }

// Hiệu ứng mở thư
function openLetterFold(){
  const letter = document.getElementById('letter');
  const finalGift = document.getElementById('finalGift');
  letter.style.transform = 'rotateX(-90deg)';
  finalGift.style.opacity = 0;
  setTimeout(()=>{letter.style.transform='rotateX(0deg)';},300);
  setTimeout(()=>{finalGift.style.opacity=1;},1800);
}

// Heart particle
function startHeartParticles() {
  const canvas = document.getElementById('pinkboard');
  const context = canvas.getContext('2d');
  canvas.width = canvas.clientWidth; canvas.height = canvas.clientHeight;
  const settings = { particles: { length: 5000, duration: 4, velocity: 80, effect: -1.3, size: 8 } };

  class Point {constructor(x=0,y=0){this.x=x;this.y=y;} clone(){return new Point(this.x,this.y);} length(l){if(l===undefined) return Math.sqrt(this.x*this.x+this.y*this.y); this.normalize(); this.x*=l; this.y*=l; return this;} normalize(){const len=this.length(); this.x/=len; this.y/=len; return this;}}
  class Particle {constructor(){this.position=new Point(); this.velocity=new Point(); this.acceleration=new Point(); this.age=0;} initialize(x,y,dx,dy){this.position.x=x; this.position.y=y; this.velocity.x=dx; this.velocity.y=dy; this.acceleration.x=dx*settings.particles.effect; this.acceleration.y=dy*settings.particles.effect; this.age=0;} update(dt){this.position.x+=this.velocity.x*dt; this.position.y+=this.velocity.y*dt; this.velocity.x+=this.acceleration.x*dt; this.velocity.y+=this.acceleration.y*dt; this.age+=dt;} draw(ctx,img){const ease=t=>(--t)*t*t+1; const size=img.width*ease(this.age/settings.particles.duration); ctx.globalAlpha=1-this.age/settings.particles.duration; ctx.drawImage(img,this.position.x-size/2,this.position.y-size/2,size,size);}}
  class ParticlePool {constructor(len){this.particles=new Array(len).fill(0).map(()=>new Particle()); this.firstActive=0; this.firstFree=0;} add(x,y,dx,dy){this.particles[this.firstFree].initialize(x,y,dx,dy); this.firstFree++; if(this.firstFree==this.particles.length)this.firstFree=0; if(this.firstActive==this.firstFree)this.firstActive++; if(this.firstActive==this.particles.length)this.firstActive=0;} update(dt){if(this.firstActive<this.firstFree){for(let i=this.firstActive;i<this.firstFree;i++) this.particles[i].update(dt);} if(this.firstFree<this.firstActive){for(let i=this.firstActive;i<this.particles.length;i++) this.particles[i].update(dt); for(let i=0;i<this.firstFree;i++) this.particles[i].update(dt);} while(this.particles[this.firstActive].age>=settings.particles.duration && this.firstActive!=this.firstFree){this.firstActive++; if(this.firstActive==this.particles.length)this.firstActive=0;}} draw(ctx,img){if(this.firstActive<this.firstFree){for(let i=this.firstActive;i<this.firstFree;i++) this.particles[i].draw(ctx,img);} if(this.firstFree<this.firstActive){for(let i=this.firstActive;i<this.particles.length;i++) this.particles[i].draw(ctx,img); for(let i=0;i<this.firstFree;i++) this.particles[i].draw(ctx,img);}}}
  
  const particlePool = new ParticlePool(settings.particles.length);
  function pointOnHeart(t){return new Point(160*Math.pow(Math.sin(t),3),130*Math.cos(t)-50*Math.cos(2*t)-20*Math.cos(3*t)-10*Math.cos(4*t)+25);}
  const image = (()=>{const c=document.createElement('canvas'),ctx=c.getContext('2d'); c.width=settings.particles.size; c.height=settings.particles.size; ctx.beginPath(); let t=-Math.PI; let pt=pointOnHeart(t); ctx.moveTo(settings.particles.size/2+pt.x*settings.particles.size/350,settings.particles.size/2-pt.y*settings.particles.size/350); while(t<Math.PI){t+=0.01; pt=pointOnHeart(t); ctx.lineTo(settings.particles.size/2+pt.x*settings.particles.size/350,settings.particles.size/2-pt.y*settings.particles.size/350);} ctx.closePath(); ctx.fillStyle='#f50b02'; ctx.fill(); const img=new Image(); img.src=c.toDataURL(); return img;})();
  
  let lastTime = null;
  function render(now){
    requestAnimationFrame(render);
    if(!lastTime) lastTime=now;
    const dt=(now-lastTime)/1000; lastTime=now;
    context.clearRect(0,0,canvas.width,canvas.height);
    const particleRate = settings.particles.length/settings.particles.duration;
    const amount = particleRate*dt;
    for(let i=0;i<amount;i++){const pos=pointOnHeart(Math.PI-2*Math.PI*Math.random()); const dir=pos.clone().length(settings.particles.velocity); particlePool.add(canvas.width/2+pos.x,canvas.height/2-pos.y,dir.x,-dir.y);}
    particlePool.update(dt);
    particlePool.draw(context,image);
  }
  render();
}

document.getElementById('heartBtn')?.addEventListener('click', ()=>{
  go('heartEffect');
  startHeartParticles();
  setTimeout(()=>go('gift'),5000);
});
</script>

</body>
</html>
