 <!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Acesso GV</title>
  <style>
    /* Página inicial - Tela de senha */
    body {
      margin: 0; padding: 0;
      font-family: Arial, sans-serif;
      background-color: #000000; /* Preto */
      color: #00ff00; /* Verde brilhante */
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
    }
    #login-box {
      background: #000000;
      border: 2px solid #00ff00;
      padding: 30px 40px;
      border-radius: 12px;
      text-align: center;
      width: 320px;
      box-shadow: 0 0 20px #00ff00;
    }
    #login-box h2 {
      font-size: 2.5rem;
      margin-bottom: 15px;
      position: relative;
      padding-top: 10px;
    }
    /* Ícone ponto de interrogação em cima */
    #login-box h2::before {
      content: "?";
      display: block;
      font-size: 4rem;
      color: #00ff00;
      margin-bottom: 10px;
      font-weight: bold;
    }
     #senha  {
      width: 90%;
      padding: 12px;
      font-size: 1.2rem;
      border: 2px solid #00ff00;
      background: black;
      color: #00ff00;
      border-radius: 6px;
      outline: none;
    }
    #senha::placeholder {
      color: #00ff00;
      opacity: 0.6;
    }
    button {
      margin-top: 20px;
      padding: 12px 30px;
      font-size: 1.2rem;
      color: #000;
      background-color: #00ff00;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #33ff33;
    }

    /* GVNews e GVCrypto - fundo preto + azul marinho + dourado */
    #gvnews-page, #gvcrypto-page {
      display: none;
      max-width: 900px;
      margin: 30px auto;
      background: #001122; /* azul marinho escuro */
      border-radius: 12px;
      padding: 25px 30px;
      color: #f5deb3; /* dourado claro */
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      box-shadow: 0 0 20px #daa520; /* sombra dourada */
    }
    #gvnews-page h1, #gvcrypto-page h1 {
      font-weight: 900;
      font-size: 2.5rem;
      color: #daa520; /* dourado */
      border-bottom: 3px solid #daa520;
      padding-bottom: 10px;
      margin-bottom: 25px;
    }

    /* GVNews - notícias */
    #relogio {
      font-weight: bold;
      font-size: 1.4rem;
      margin-bottom: 20px;
      color: #90ee90; /* verde claro */
      text-align: center;
      font-family: 'Courier New', monospace;
    }
    #feed-noticias {
      background-color: #002244; /* azul marinho mais claro */
      padding: 15px;
      border-radius: 10px;
      max-height: 200px;
      overflow-y: auto;
      margin-bottom: 30px;
      color: #f5deb3;
      font-size: 1rem;
      box-shadow: inset 0 0 10px #daa520;
    }
    .noticia-item {
      border-bottom: 1px solid #daa520;
      padding: 8px 0;
    }
    .article {
      margin-bottom: 30px;
      border-bottom: 1px solid #daa520;
      padding-bottom: 15px;
    }
    .article h2 {
      color: #daa520;
      margin: 0 0 10px 0;
    }
    .article p {
      color: #f5deb3;
      line-height: 1.5;
      font-size: 1.1rem;
    }

    /* GVCrypto - centro de investimentos */
    #gvcrypto-page h2 {
      color: #daa520;
      margin-bottom: 15px;
      font-weight: 700;
    }
    .section {
      margin-bottom: 25px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      background: #002244;
      box-shadow: 0 0 8px #daa520 inset;
      border-radius: 8px;
      overflow: hidden;
    }
    th, td {
      padding: 10px 15px;
      border: 1px solid #daa520;
      text-align: center;
      color: #f5deb3;
      font-weight: 600;
      font-size: 1rem;
    }
    th {
      background-color: #003366;
    }
    .positive {
      color: #00ff00; /* verde */
      font-weight: bold;
    }
    .negative {
      color: #ff4500; /* vermelho alaranjado */
      font-weight: bold;
    }
  </style>
</head>
<body>

  <!-- Página inicial com senha -->
  <div id="login-box">
    <h2>Digite sua senha para acessar</h2>
    <input type="password" id="senha" placeholder="Senha aqui" />
    <br />
    <button onclick="verificarSenha()">Entrar</button>
  </div>

  <!-- GVNews (senha GVNotícias) -->
  <div id="gvnews-page">
    <h1>GVNews - Últimas Notícias</h1>
    <div id="relogio">Carregando hora...</div>

    <div id="feed-noticias"></div>

    <div class="article">
      <h2>Economia cresce 2% no último trimestre</h2>
          <p>O PIB brasileiro apresentou crescimento acima do esperado, impulsionado pelo aumento nas exportações...</p>    
    </div>

    <div class="article">
      <h2>Vacinação contra a gripe começa em todo o país</h2>
            <p>Autoridades de saúde iniciam campanha anual de vacinação para proteger a população contra a gripe sazonal...</p>      
    </div>

    <div class="article">
      <h2>Novas medidas de segurança para o trânsito são anunciadas</h2>
       <p>O governo federal anunciou novas regras para aumentar a segurança nas rodovias e reduzir acidentes...</p> 
    </div>
 <Div.> </Div.> </Div.>

  <!-- GVCrypto (senha GVCrypto) -->
 <divid="gvcrypto-page"> <Div. id="gvcrypto-page">
     <H1>GVCrypto - Centro de Investimentos</H1> <H1>GVCrypto - Centro de Investimentos</H1>

    <div class="section">
      <h2>Bolsas de Valores</h2>
      <table>
        <thead>
     <tr> 
             <th>Bolsa</th> 
     <a>Índice</a> 
             <th>Valor Atual</th> 
             <th>Variação</th> 
     </tr> 
     <aaaia> 
     <tbody id="caixa-mesa"></corpo> 
     </Tabela> 
    </div>

    <div class="seção">
       <h2>Criptomoedas</h2> 
     <Tabela> 
     <aa cabeça> 
     <tr> 
             <th>Moeda</th> 
             <th>Preço Atual (USD)</th> 
             <th>Variação 24h</th> 
     </tr> 
     <aaaia> 
     <tbody id="cripto-mesa-corpo"></corpo> 
     </Tabela> 
    </div>
 <Div.> </Div.></Div.> 

 <Roteiro> <Roteiro><Roteiro>
         const senhaGVNews = "GVNotícias"; const senhaGVNews = "GVNotícias";    
        const senhaGVCrypto = "GVCrypto";    

      function verificarSenha() { function verificarSenha() {
     entrada de     

    if(input === senhaNotícias) {    
      mostrar mostrar     
           } else if(input === senhaGVCrypto) {      } else if(input === senhaGVCrypto) {    
              mostrarGVCrypto();         mostrarGVCrypto();     
      } mais { } mais {     
              alert('Senha incorreta! Tente novamente.');         alert('Senha incorreta! Tente novamente.');     
         }   
      }  

       // Funções para mostrar páginas e esconder login // Funções para mostrar páginas e esconder login 
     função     
 documento. getElementById('login-box').style.display = 'nenhum'; getElementById('login-box').style.display = 'nenhum';
 documento. getElementById('gvnews-page').style.display = 'bloqueio'; getElementById('gvnews-page').style.display = 'bloco';
            iniciarRelogio();      
       iniciar o       
       }   

     função mostrar     
 documento. getElementById('login-box').style.display = 'nenhum'; getElementById('login-box').style.display = 'nenhum';
 documento. getElementById('gvcrypto-page').style.display = 'bloqueio'; getElementById('gvcrypto-page').style.display = 'bloco';
            carregarDadosInvestimentos();      
      }  

 // GVNews - relógio 
       função       
     função atualizarHora() {     
              const agora = new Date();      
               const horas = String(agora.getHours()).padStart(2, '0');       
          const minutos = String(agora.getMinutes()).padStart(2, '0');  CriptoPortal  com notícias e centros de investimentoCriptoPortal  com notícias e centros de investimento   (2, '0')    CriptoPortal  com notícias e centros de investimentoCriptoPortal  com notícias e centros de investimento   
