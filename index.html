<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Desktop</title>

<style>
body {
  margin: 0;
  font-family: Arial;
  background: linear-gradient(#0a0a0a, #1a1a1a);
  height: 100vh;
  overflow: hidden;
  color: white;
}

/* Desktop */
.desktop {
  padding: 20px;
  display: grid;
  grid-template-columns: repeat(6, 80px);
  gap: 20px;
}
.icon { text-align: center; cursor: pointer; }
.icon span { font-size: 32px; }
.icon p { font-size: 12px; }

/* Barra */
.taskbar {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 50px;
  background: rgba(20,20,20,0.95);
  display: flex;
  align-items: center;
  padding: 0 10px;
}

.start-btn { cursor: pointer; font-size: 20px; }

.search {
  margin-left: 10px;
  background: #2a2a2a;
  border-radius: 20px;
  padding: 5px 10px;
  border: none;
  color: white;
}

.task-icons {
  display: flex;
  gap: 10px;
  margin-left: 15px;
}

.task-icons span {
  cursor: pointer;
}

.clock { margin-left: auto; }

/* Menu iniciar */
.start-menu {
  position: fixed;
  bottom: 60px;
  left: 10px;
  width: 220px;
  background: #1e1e1e;
  padding: 10px;
  display: none;
  border-radius: 10px;
}
.start-menu div {
  padding: 8px;
  cursor: pointer;
}
.start-menu div:hover {
  background: #333;
}

/* Janelas */
.window {
  position: absolute;
  width: 320px;
  height: 260px;
  background: #1e1e1e;
  border-radius: 10px;
  display: none;
  flex-direction: column;
  animation: abrir 0.2s ease;
}

@keyframes abrir {
  from { transform: scale(0.8); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

.title-bar {
  background: #333;
  padding: 5px;
  display: flex;
  justify-content: space-between;
  cursor: move;
}

.close { cursor: pointer; }

/* Conteúdo */
.content {
  flex: 1;
  padding: 10px;
}

/* Bloco de notas */
textarea {
  width: 100%;
  height: 100%;
  background: black;
  color: white;
  border: none;
  resize: none;
}
</style>
</head>

<body>

<!-- Desktop -->
<div class="desktop">
  <div class="icon" onclick="abrir('notas')">
    <span>📝</span><p>Notas</p>
  </div>

  <div class="icon" onclick="abrir('browser')">
    <span>🌐</span><p>Navegador</p>
  </div>

  <div class="icon" onclick="abrir('files')">
    <span>📁</span><p>Arquivos</p>
  </div>
</div>

<!-- Menu iniciar -->
<div class="start-menu" id="menu">
  <div onclick="abrir('notas')">📝 Notas</div>
  <div onclick="abrir('browser')">🌐 Navegador</div>
  <div onclick="abrir('files')">📁 Arquivos</div>
</div>

<!-- Janelas -->

<div class="window" id="notas" style="top:100px; left:100px;">
  <div class="title-bar">
    <span>📝 Bloco de Notas</span>
    <span class="close" onclick="fechar('notas')">❌</span>
  </div>
  <div class="content">
    <textarea id="text"></textarea>
  </div>
</div>

<div class="window" id="browser" style="top:150px; left:200px;">
  <div class="title-bar">
    <span>🌐 Navegador</span>
    <span class="close" onclick="fechar('browser')">❌</span>
  </div>
  <div class="content">
    <p>Simulação de navegador 👀</p>
  </div>
</div>

<div class="window" id="files" style="top:120px; left:250px;">
  <div class="title-bar">
    <span>📁 Arquivos</span>
    <span class="close" onclick="fechar('files')">❌</span>
  </div>
  <div class="content">
    <p>📄 arquivo.txt</p>
    <p>📄 notas.md</p>
  </div>
</div>

<!-- Barra -->
<div class="taskbar">
  <div class="start-btn" onclick="toggleMenu()">🪟</div>
  <input class="search" placeholder="Pesquisar...">

  <div class="task-icons" id="apps"></div>

  <div class="clock" id="clock"></div>
</div>

<script>
// abrir janela
function abrir(id) {
  document.getElementById(id).style.display = "flex";

  let apps = document.getElementById("apps");
  if (!document.getElementById("task-" + id)) {
    let icon = document.createElement("span");
    icon.innerText = "🟦";
    icon.id = "task-" + id;
    icon.onclick = () => abrir(id);
    apps.appendChild(icon);
  }
}

// fechar janela
function fechar(id) {
  document.getElementById(id).style.display = "none";
}

// menu iniciar
function toggleMenu() {
  let m = document.getElementById("menu");
  m.style.display = m.style.display === "block" ? "none" : "block";
}

// relógio
function clock() {
  let d = new Date();
  document.getElementById("clock").innerText =
    d.getHours().toString().padStart(2,'0') + ":" +
    d.getMinutes().toString().padStart(2,'0');
}
setInterval(clock,1000);
clock();

// salvar bloco de notas
let txt = document.getElementById("text");
txt.value = localStorage.getItem("notas") || "";
txt.addEventListener("input", () => {
  localStorage.setItem("notas", txt.value);
});

// arrastar janelas
document.querySelectorAll(".window").forEach(win => {
  let isDown = false, offsetX, offsetY;
  const bar = win.querySelector(".title-bar");

  bar.addEventListener("mousedown", e => {
    isDown = true;
    offsetX = e.clientX - win.offsetLeft;
    offsetY = e.clientY - win.offsetTop;
  });

  document.addEventListener("mouseup", () => isDown = false);

  document.addEventListener("mousemove", e => {
    if (isDown) {
      win.style.left = e.clientX - offsetX + "px";
      win.style.top = e.clientY - offsetY + "px";
    }
  });
});
</script>

</body>
</html>
