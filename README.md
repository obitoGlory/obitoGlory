# 🌌 obitoGlory

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>obitoGlory - Web Developer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/@lucide/web/dist/umd/lucide.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600;700&display=swap');
        * { margin:0; padding:0; box-sizing:border-box; font-family:'JetBrains Mono', monospace; }
        body { background:linear-gradient(135deg,#0f2027,#203a43,#2c5364); color:#e2e8f0; min-height:100vh; padding:2rem; }
        .container{ max-width:1200px; margin:0 auto; }
        .card-3d{ transform-style:preserve-3d; perspective:1000px; transition:all .3s ease; }
        .card-3d:hover{ transform:translateY(-5px) rotateX(5deg); box-shadow:0 20px 30px rgba(0,0,0,.3); }
        .typing-animation{ overflow:hidden; border-right:2px solid #fff; white-space:nowrap; animation:typing 4s steps(40,end),blink-caret .75s step-end infinite; }
        @keyframes typing{ from{width:0} to{width:100%} }
        @keyframes blink-caret{ from,to{border-color:transparent} 50%{border-color:#fff} }
        .skill-icon{ transition:.3s; filter:grayscale(30%); }
        .skill-icon:hover{ transform:scale(1.2) translateY(-5px); filter:grayscale(0); }
        .github-stats{ background:rgba(255,255,255,.05); backdrop-filter:blur(10px); border-radius:12px; padding:1.5rem; transition:.3s; }
        .github-stats:hover{ background:rgba(255,255,255,.1); transform:translateY(-3px); }
        .snake-animation{ filter:drop-shadow(0 0 5px rgba(0,0,0,.3)); }
        .gradient-text{ background:linear-gradient(90deg,#63b3ed,#4299e1,#3182ce); -webkit-background-clip:text; -webkit-text-fill-color:transparent; background-size:200% auto; animation:gradient 3s linear infinite; }
        @keyframes gradient{ 0%{background-position:0% center;} 100%{background-position:200% center;} }
        .neon-border{ border:1px solid transparent; background:linear-gradient(135deg,#0f2027,#203a43,#2c5364) padding-box,linear-gradient(45deg,#63b3ed,#4299e1,#3182ce) border-box; }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="text-center mb-12">
            <h1 class="text-5xl md:text-6xl font-bold mb-4 gradient-text">obitoGlory</h1>
            <div class="neon-border rounded-xl p-6 shadow-2xl">
                <p class="text-xl md:text-2xl mb-2">javascript | html | css | linux(pop!_os)</p>
                <div class="typing-animation max-w-max mx-auto text-lg md:text-xl">
                    Web Developer & Linux Enthusiast
                </div>
            </div>
        </div>
        <!-- About -->
        <div class="card-3d neon-border rounded-xl p-6 mb-12">
            <h2 class="text-3xl font-bold mb-6 text-center gradient-text">Tentang Saya</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div>
                    <p class="text-lg mb-4">Saya adalah seorang web developer fokus pada JavaScript, HTML, dan CSS.</p>
                    <p class="text-lg mb-4">Menggunakan Pop!_OS sebagai OS utama.</p>
                    <p class="text-lg">Masih belajar tapi semangat bikin project web yang menarik 🚀</p>
                </div>
                <div class="flex justify-center items-center">
                    <img src="https://files.catbox.moe/za3vvd.gif" alt="Coding Animation" class="rounded-xl max-w-full h-auto shadow-lg">
                </div>
            </div>
        </div>
        <!-- Skills -->
        <div class="card-3d neon-border rounded-xl p-6 mb-12">
            <h2 class="text-3xl font-bold mb-8 text-center gradient-text">Skills & Tools</h2>
            <div class="flex flex-wrap justify-center gap-8">
                <div class="skill-icon text-center"><div class="w-16 h-16 mx-auto mb-2 bg-blue-500 rounded-xl flex items-center justify-center"><i data-lucide="code-2" class="text-white w-10 h-10"></i></div><span>JavaScript</span></div>
                <div class="skill-icon text-center"><div class="w-16 h-16 mx-auto mb-2 bg-orange-500 rounded-xl flex items-center justify-center"><i data-lucide="html5" class="text-white w-10 h-10"></i></div><span>HTML5</span></div>
                <div class="skill-icon text-center"><div class="w-16 h-16 mx-auto mb-2 bg-blue-700 rounded-xl flex items-center justify-center"><i data-lucide="css3" class="text-white w-10 h-10"></i></div><span>CSS3</span></div>
                <div class="skill-icon text-center"><div class="w-16 h-16 mx-auto mb-2 bg-yellow-500 rounded-xl flex items-center justify-center"><i data-lucide="cpu" class="text-white w-10 h-10"></i></div><span>Linux</span></div>
            </div>
        </div>
        <!-- Projects -->
        <div class="card-3d neon-border rounded-xl p-6 mb-12">
            <h2 class="text-3xl font-bold mb-8 text-center gradient-text">Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-gray-800 rounded-xl p-4"><h3 class="text-xl font-semibold mb-2">Personal Website</h3><p>Website dengan JS, HTML, dan CSS.</p></div>
                <div class="bg-gray-800 rounded-xl p-4"><h3 class="text-xl font-semibold mb-2">Custom Linux Setup</h3><p>Optimasi Pop!_OS untuk dev & gaming.</p></div>
                <div class="bg-gray-800 rounded-xl p-4"><h3 class="text-xl font-semibold mb-2">Web Playground</h3><p>Eksperimen animasi CSS & interaktif JS.</p></div>
            </div>
        </div>
        <!-- GitHub Snake -->
        <div class="card-3d neon-border rounded-xl p-6 mb-12">
            <h2 class="text-3xl font-bold mb-4 text-center gradient-text">GitHub Contributions</h2>
            <div class="snake-animation bg-gray-800 rounded-xl p-4">
                <img src="https://raw.githubusercontent.com/obitoGlory/obitoGlory/output/github-contribution-grid-snake.svg" alt="Snake animation" class="w-full">
            </div>
        </div>
        <!-- Connect -->
        <div class="text-center">
            <h2 class="text-3xl font-bold mb-6 gradient-text">Terhubung</h2>
            <a href="https://github.com/obitoGlory" class="inline-flex items-center bg-gray-800 hover:bg-gray-700 text-white font-bold py-3 px-6 rounded-xl transition-all">
                <i data-lucide="github" class="w-5 h-5 mr-2"></i> GitHub Saya
            </a>
        </div>
    </div>
    <script>
        lucide.createIcons();
        const texts=["halo, aku obitoGlory ✨","ngoprek javascript, html, css","ngulik linux pop!_os tiap hari","ngoding project web 🚀"];
        let i=0,j=0,current='',del=false,speed=100;
        function type(){
          const el=document.querySelector('.typing-animation');
          if(!el)return;
          if(del){current=texts[i].substring(0,j-1);j--;}else{current=texts[i].substring(0,j+1);j++;}
          el.textContent=current;
          let delay=del?speed/2:speed;
          if(!del && current===texts[i]){delay=2000;del=true;}
          else if(del && current===''){del=false;i++;if(i>=texts.length)i=0;delay=500;}
          setTimeout(type,delay);
        }
        document.addEventListener('DOMContentLoaded',type);
    </script>
</body>
</html>
