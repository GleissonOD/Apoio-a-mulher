# Minuto-de-apoio-aa-mulheres
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Minuto de Apoio</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #ffe6f0;
      color: #333;
      text-align: center;
      padding: 30px;
    }

    h1 {
      color: #c2185b;
      margin-bottom: 20px;
    }

    .caixa {
      background: #fff;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 0 10px #ccc;
      max-width: 600px;
      margin: auto;
    }

    p#frase {
      font-size: 1.2em;
      margin-bottom: 15px;
    }

    button {
      padding: 10px 20px;
      background-color: #c2185b;
      color: #fff;
      border: none;
      border-radius: 5px;
      font-size: 1em;
      cursor: pointer;
      transition: background-color 0.3s;
    }

    button:hover {
      background-color: #a3154e;
    }

    hr {
      margin: 25px 0;
    }

    .links a {
      display: block;
      margin: 8px 0;
      color: #c2185b;
      text-decoration: none;
      font-weight: bold;
    }

    .links a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <h1>Minuto de Apoio</h1>

  <div class="caixa">
    <p id="frase">Você é mais forte do que imagina.</p>
    <button onclick="novaFrase()">Nova Frase</button>

    <hr>

    <p><strong>Dica de bem-estar:</strong> Cuide da sua mente como cuida do seu corpo.</p>

    <hr>

    <div class="links">
      <h3>Links Úteis</h3>
      <a href="https://www.cvv.org.br/" target="_blank">CVV - Apoio Emocional</a>
      <a href="https://www.gov.br/mdh/pt-br/ondemulher" target="_blank">Central de Atendimento à Mulher</a>
      <a href="https://play.google.com/store/apps/details?id=com.meditopia.android&hl=pt_BR" target="_blank">App de Meditação</a>
    </div>
  </div>

  <script>
  const frases = [
    "Você é capaz de grandes realizações.",
      "Sua voz importa.",
      "Confie no seu valor.",
      "Você não está sozinha.",
      "A sua força está no seu coração.",
      "Permita-se descansar — sem culpa, sem peso.",
      "Você merece amor e respeito.",
      "Continue. Mesmo devagar, você está avançando.",
      "Você é suficiente.",
      "Sua coragem inspira.",
      "Seja gentil com você mesma.",
      "Você pode mudar o mundo à sua maneira.",
      "Lute pelos seus sonhos.",
      "Você é luz, mesmo em dias nublados.",
      "Acredite: você já venceu muito.",
      "Seja você. Sempre.",
      "Você merece o melhor da vida.",
      "Nunca duvide do seu poder.",
      "Você é única e isso é sua força.",
      "Ouça sua intuição: ela é sábia.",
      "Seu sorriso ilumina caminhos.",
      "Você é digna de tudo o que deseja.",
      "Cada dia é uma nova chance.",
      "Não se compare. Você é especial do seu jeito.",
      "Resiliência é o seu superpoder.",
      "Você inspira mais do que imagina.",
      "Seja sua maior aliada.",
      "Não se cale diante da injustiça.",
      "Sua presença faz diferença.",
      "Não carregue culpas que não são suas.",
      "Você é amor em movimento.",
      "Não há limites para quem acredita.",
      "Seu corpo é sua casa: cuide com carinho.",
      "Você é parte da mudança.",
      "Permita-se ser feliz agora.",
      "Errar faz parte do caminho.",
      "Tudo bem não estar bem.",
      "Você não precisa dar conta de tudo.",
      "Respire fundo. Você está indo bem.",
      "Você é mais do que aparenta.",
      "O mundo precisa do seu brilho.",
      "Valorize suas conquistas, por menores que pareçam.",
      "Você é esperança para outras mulheres.",
      "Nunca é tarde para recomeçar.",
      "Você tem o direito de dizer não.",
      "Cuidar de si não é egoísmo, é amor-próprio.",
      "Você transforma o que toca.",
      "Você merece paz.",
      "Seu sentimento é válido.",
      "Você tem direito a ocupar espaços.",
      "Suas ideias são importantes.",
      "Você pode e vai conseguir.",
      "Tudo começa com um passo.",
      "A sua existência já é resistência.",
      "Você é feita de possibilidades.",
      "Você tem força ancestral.",
      "Não tenha medo de brilhar.",
      "Você não precisa ser perfeita.",
      "Seu tempo é sagrado.",
      "Você é potência.",
      "Você está crescendo mesmo quando parece parada.",
      "Você tem valor, mesmo quando não se sente assim.",
      "Seu amor-próprio muda tudo.",
      "Você é capaz de reinventar sua história.",
      "Seu cansaço é válido. Descanse.",
      "Você não precisa agradar a todos.",
      "Você pode ser forte e sensível ao mesmo tempo.",
      "Você merece ser ouvida.",
      "Você é inspiração para alguém.",
      "Você é completa como é.",
      "Sua jornada é só sua.",
      "Você é feita de coragem e doçura.",
      "Você é seu maior projeto.",
      "Continue mesmo com medo.",
      "Você é dona do seu destino.",
      "Você tem direito à felicidade.",
      "A sua luta é legítima.",
      "Você floresce mesmo nas dificuldades.",
      "Sua história importa.",
      "Você não é o que te fizeram acreditar.",
      "Você é a mudança que espera.",
      "Permita-se evoluir com leveza.",
      "Você já venceu ao continuar.",
      "Você tem a força das que vieram antes.",
      "Você merece se amar todos os dias.",
      "Seja seu próprio abrigo.",
      "Você tem tudo o que precisa dentro de si.",
      "Você é digna de respeito em qualquer lugar.",
      "Sua sensibilidade é uma força.",
      "A sua liberdade começa com autocuidado.",
      "Você inspira outras só por existir.",
      "Você merece carinho, inclusive de si mesma.",
      "Você tem um brilho que ninguém apaga.",
      "Permita-se dizer 'basta'.",
      "Você não está sozinha. Muitas te apoiam.",
      "Você é um universo inteiro.",
      "Confie na sua jornada.",
      "Você é parte de algo maior.",
      "O amor próprio é o início de tudo.",
      "Você é mais que seus erros.",
      "Você merece segurança, respeito e amor.",
      "Sua existência é resistência.",
      "Sua presença já muda o ambiente.",
      "Você é necessária nesse mundo.",
      "Você vale muito. Nunca se esqueça.",
      "Você tem o direito de existir plenamente.",
      "Você é luz onde passa.",
      "Você merece ser feliz do seu jeito.",
      "Você pode ser o que quiser.",
      "Você não precisa provar nada para ninguém.",
      "Você é suficiente, mesmo fora dos padrões.",
      "Seu corpo é lindo como é.",
      "Crescer não precisa doer — cuide de si no processo.",
      "Você merece ser respeitada em todas as fases.",
      "Não aceite menos do que você merece.",
      "Você tem valor mesmo em silêncio.",
      "Sua vida importa.",
      "Você é forte, mesmo quando chora.",
      "Você é feita de estrelas.",
      "Você é livre para mudar de ideia.",
      "Você é capaz de romper ciclos.",
      "Você pode descansar sem culpa.",
      "Você é corajosa só por continuar.",
      "Você pode sonhar alto.",
      "Seu bem-estar é prioridade.",
      "Você pode escolher a leveza.",
      "Você está viva, e isso já é vitória.",
      "Você é seu lar.",
      "Você é suficiente mesmo nos dias difíceis.",
      "Você é sua melhor companhia.",
      "Você é amor próprio em construção.",
      "Seu brilho incomoda quem vive na sombra.",
      "Você merece ser celebrada todos os dias.",
      "A força feminina é revolucionária.",
      "Você pode dizer ‘sim’ para você.",
      "Você não é drama, é intensidade.",
      "Você pode se reinventar hoje.",
      "Você não precisa ser forte o tempo todo.",
      "Você é luz até quando duvida disso.",
      "Você é linda de alma e corpo.",
      "Você tem o direito de mudar de caminho.",
      "Você merece ser cuidada com carinho.",
      "Você é bem-vinda no mundo.",
      "Você é raiz e flor ao mesmo tempo.",
      "Você é mais que aparência.",
      "Você pode ter sucesso e descanso.",
      "Sua dor não te define.",
      "Você é farol em noite escura.",
      "Você é feita para voar, não para se limitar.",
      "Você é presença, não ausência.",
      "Você é verdade, mesmo que não entendam.",
      "Você pode dizer o que sente.",
      "Você pode começar de novo agora.",
      "Cuide da sua mente como cuida do seu corpo.",
      "Paz é prioridade, não luxo.",
      "Você não precisa se apressar. O seu tempo é sagrado.",
      "Descansar também é um ato de coragem.",
      "Sentir é humano. Negar-se não te faz mais forte.",
      "Acolha suas emoções, até as mais confusas.",
      "Você tem permissão para se colocar em primeiro lugar.",
      "Você merece um trabalho que te respeite.",
      "O mundo profissional precisa da sua autenticidade.",
      "Você tem competência, não se minimize.",
      "Seu talento não depende da validação de ninguém.",
      "Seja firme, mesmo que te chamem de difícil.",
      "Você pode ser ambiciosa e gentil.",
      "Empreender sua vida também é sucesso.",
      "Suas metas importam — grandes ou pequenas.",
      "Relacionamentos saudáveis começam com amor-próprio.",
      "Você merece reciprocidade, não migalhas.",
      "Dizer não também é um ato de amor.",
      "Amor não deve doer, deve somar.",
      "Você não precisa se diminuir para caber em alguém.",
      "Só fique onde seu coração cabe inteiro.",
      "Se não te valoriza, não merece espaço.",
      "Você está exatamente onde deveria estar para crescer.",
      "Sua caminhada não precisa seguir o mapa de ninguém.",
      "A dúvida também ensina.",
      "Você pode recomeçar tantas vezes quanto quiser.",
      "A mulher que você é hoje honra todas as que já foi.",
      "Cada escolha que te respeita é um passo à frente.",
      "Não há vergonha em mudar de direção."

    ];

    function novaFrase() {
      const index = Math.floor(Math.random() * frases.length);
      document.getElementById("frase").textContent = frases[index];
    }
  </script>

</body>
</html>
