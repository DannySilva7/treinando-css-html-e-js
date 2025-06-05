<!DOCTYPE html>
 <html lang="pt-br">
    <head>
     <meta charset="UTF-8">
        <title>O próximo nível não é técnico. É psicológico.</title>
        <style>
           html {
  scroll-behavior: smooth;
}
 html, body {
  height: 100%;
  margin: 0;
  padding: 0;
}
.card {
  opacity: 0;
  transform: translateY(30px);
  transition: all 0.6s ease;
}

.card.animar {
  opacity: 1;
  transform: translateY(0);
}
.card.animar {
  box-shadow: 0 0 15px rgba(255, 0, 183, 0.4);
}
           body 
       {
  margin: 0;
  padding: 0;
  min-height: 100vh;
  background: linear-gradient(-45deg, #9375db, #6f5a91, #48284d, #ff00b7);
  background-size: 400% 400%;
  animation: animarFundo 15s ease infinite;
  color: #f0f0f0;
  font-family: Arial, sans-serif;
  padding: 30px;
  overflow-x: hidden;
}

@keyframes animarFundo {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

 h1 {
      color: #f1f3f1;
      text-shadow: 1px 1px 5px #6f5a91;
    }
 
    h2 {
      color: #ff00b7;
    }

    p {
      background-color: #48284d;
      padding: 20px;
      border-radius: 10px;
      line-height: 1.6;
      opacity: 1;
      transition: opacity 1s ease-in-out;
      margin-top: 20px;
    }
    .oculto {
      opacity: 0;
      height: 0;
      overflow: hidden;
    }
    button {
        margin-top: 20px;
        padding: 10px 20px;
        font-size: 16px;
        border: none;
        border-radius: 8px;
        background-color: #ff00b7;
        color: white;
        cursor: pointer;
        transition: 0.3s;
      }

      button:hover {
        background-color: #ac3b90;
      }

      #mensagem {
        margin-top: 20px;
        background-color: #1b1919;
        padding: 20px;
        border-radius: 10px;
        color: #f1b3df;
        font-style: italic;
        display: none; /* Inicialmente oculto */
      }
  header {
      background-color: #6f5a91;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      padding: 15px 30px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
      z-index: 1000;
    }

    nav a {
      margin: 0 15px;
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ff00b7;
    }

    section {
      padding: 30px 0;
    }
    #diario {
  margin-top: 60px;
  padding: 40px 20px;
}

#diario h2 {
  text-align: center;
  color: #ff00b7;
  margin-bottom: 30px;
  font-size: 28px;
}

.card {
  background-color: #321c4f;
  border-radius: 12px;
  padding: 20px;
  margin-bottom: 20px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  transition: transform 0.3s ease, background-color 0.3s;
}

.card:hover {
  transform: translateY(-5px);
  background-color: #482c6c;
}

.card h3 {
  margin-top: 0;
  color: #ffd6f5;
}

.card p {
  color: #f0f0f0;
  line-height: 1.6;
}
#fundoCanvas {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1; /* Fica atrás de tudo */
  background: #0d0b19; /* Fundo escuro, como o espaço */
}
  </style>
</head>
<body>
   <canvas id="fundoCanvas"></canvas>
  <header>
    <nav>
      <a href="#inicio">Início</a>
      <a href="#sobre">Sobre</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

   <section id="inicio"></section>
    <h1><em>Tudo começo aqui...</em></h1>
    <h2>Vamos criar este lugar juntos!...</h2>
        <p>
           <em>
                Este é o início de uma jornada.<br />
  Cada linha escrita aqui é mais do que código é um passo rumo à liberdade de criar, aprender e evoluir.<br>
  Todo grande desenvolvedor começou com algo simples.<br>
  O importante não é onde você começa, mas a coragem de continuar.<br>
  Continue. Construa. Cresça.
            </em>
         </p>
</section>
        
<section id="sobre">
    <h2>Sobre este projeto</h2>
    <p>
      Este projeto nasceu da sua vontade de aprender e evoluir.<br>
      Ele é uma semente de um futuro onde você domina ferramentas criativas e transforma ideias em realidade. Cada linha aqui escrita é uma prova do seu comprometimento com sua própria evolução.
    </p>
      </section>
 
  <section id="contato">
    <h2>Entre em contato</h2>
    <p>Sim, você pode conversar com seu próprio código. E ele responde.</p>

  <button onclick="mostrarMensagem()">Clique aqui para o próximo passo</button>
         <div id="mensagem"></div>
    
  <button onclick="revelarParagrafos()">Mostrar mais inspiração</button> 

    <p class="oculto" id="p1"><em>Você já começou — e isso já te coloca na frente de quem só pensa, mas nunca faz.</em></p>
    <p class="oculto" id="p2"><em>O conhecimento técnico te leva até certo ponto. A mentalidade é o que te leva além.</em></p>
    <p class="oculto" id="p3"><em>Consistência silenciosa derrota talento barulhento. Mostre com ação, não com fala.</em></p>
    <p class="oculto" id="p4"><em>O próximo nível não é técnico. É psicológico. Acredite em você, mesmo quando ninguém mais acreditar.</em></p>
    </section>

<section id="portfolio">
  <h2>🔮 Meu Portfólio</h2>
  <div class="cards">
    <div class="card">
      <h3>✨ Projeto 1 Página de Boas-Vindas</h3>
      <p>Uma tela de entrada estilizada com animações e mensagens motivacionais. Foi o primeiro passo para transformar código em sentimento. Aqui nasceu o desejo de inspirar quem acessa.</p>
    </div>
    <div class="card">
      <h3>✨ Projeto 2 Botões Interativos</h3>
      <p>Criei botões que respondem ao clique com mensagens personalizadas. Cada interação é um convite ao próximo passo. Aprendi que um simples clique pode abrir portas criativas.</p>
    </div>
    <div class="card">
      <h3>✨ Projeto 3  Fundo Animado com Partículas</h3>
      <p>Desenvolvi um fundo dinâmico estilo galáxia com partículas flutuantes. Um espaço visual que representa o infinito do aprendizado e da imaginação. Técnica e estética em harmonia.</p>
    </div>
  </div>
</section>
<script>
  
  window.addEventListener("scroll", () => {
  const cards = document.querySelectorAll(".card");
  const windowAltura = window.innerHeight;

  cards.forEach(card => {
    const cardTop = card.getBoundingClientRect().top;
    if (cardTop < windowAltura - 100) {
      card.classList.add("animar");
    }
  });
});

      function mostrarMensagem() {
      const mensagem = document.getElementById("mensagem");
      mensagem.innerHTML = `
      <strong>Você deu um passo a mais!</strong> Continue explorando, aprendendo e acreditando no seu potencial.
        <p>
          Alerta: este código pode conter traços de genialidade e café.<br />
          Se você consegue ler isso, parabéns — você já sabe mais que ontem.<br />
          Pode não estar perfeito, mas está funcionando (e isso já é meio caminho andado).<br />
          Respira, salva... e bora pro próximo bug!
        </p>
      `;
      mensagem.style.display = "block";
    }

 function revelarParagrafos() {
      const paragrafos = [
        document.getElementById("p1"),
        document.getElementById("p2"),
        document.getElementById("p3"),
        document.getElementById("p4")
      ];

      paragrafos.forEach((p, i) => {
        setTimeout(() => {
          p.classList.remove("oculto");
        }, i * 1000);
      });
    }
            </script>
     <section id="diario">
  <h2>📓 Diário de Bordo (por dentro do código)</h2>

  <div class="card">
    <h3>🪄 Primeiro passo</h3>
    <p>Iniciei minha jornada. Criei meu primeiro HTML. O básico não é pequeno — é a base de tudo.</p>
  </div>

  <div class="card">
    <h3>💡 Entendendo CSS</h3>
    <p>Descobri o poder da estética. Um fundo roxo, uma sombra, um botão. Cada linha torna meu código mais meu.</p>
  </div>

  <div class="card">
    <h3>⚙️ Primeira função JS</h3>
    <p>Um clique, uma resposta. Ativei minha primeira função. Senti que podia conversar com o código.</p>
  </div>
</section>
    <script>
  const canvas = document.getElementById("fundoCanvas");
  const ctx = canvas.getContext("2d");

  function ajustarCanvas() {
    canvas.width = window.innerWidth;
    canvas.height = window.innerHeight;
  }

  window.addEventListener("resize", ajustarCanvas);
  ajustarCanvas();

  const particulas = [];

  // Criando partículas galácticas
  for (let i = 0; i < 150; i++) {
    particulas.push({
      x: Math.random() * canvas.width,
      y: Math.random() * canvas.height,
      raio: Math.random() * 2 + 1, // Partículas menores
      dx: (Math.random() - 0.5) * 0.3, // Movimentação mais lenta
      dy: (Math.random() - 0.5) * 0.3,
      cor: `hsla(${Math.random() * 360}, 100%, 80%, 0.7)` // Cores mais brilhantes (tons de azul, roxo, branco)
    });
  }

  function animar() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    particulas.forEach((p, i) => {
      // Criando as partículas
      ctx.beginPath();
      ctx.arc(p.x, p.y, p.raio, 0, Math.PI * 2);
      ctx.fillStyle = p.cor;
      ctx.fill();

      p.x += p.dx;
      p.y += p.dy;

      // Fazendo as partículas se moverem de forma fluida
      if (p.x < 0 || p.x > canvas.width) p.dx *= -1;
      if (p.y < 0 || p.y > canvas.height) p.dy *= -1;

      // Adicionando linhas entre as partículas (efeito de galáxia)
      for (let j = i + 1; j < particulas.length; j++) {
        const p2 = particulas[j];
        const dist = Math.sqrt((p.x - p2.x) ** 2 + (p.y - p2.y) ** 2);
        if (dist < 100) {
          ctx.strokeStyle = `hsla(${Math.random() * 360}, 100%, 70%, 0.1)`; // Cor suave para as linhas
          ctx.lineWidth = 0.5;
          ctx.beginPath();
          ctx.moveTo(p.x, p.y);
          ctx.lineTo(p2.x, p2.y);
          ctx.stroke();
        }
      }
    });

    requestAnimationFrame(animar);
  }

  animar();
</script>
   </script>
  </body>
 </html>
