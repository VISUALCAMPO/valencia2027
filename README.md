<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PLANO GRANDIOSO — Daniel | 2025–2027</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@1,400&display=swap');

  :root {
    --ink: #1a1510;
    --parchment: #f7f3ec;
    --gold: #c49a2e;
    --gold-light: #e8c96a;
    --rust: #8b3a1e;
    --deep: #1e2d40;
    --sage: #4a6741;
    --accent: #c49a2e;
    --line: rgba(196,154,46,0.25);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--parchment);
    color: var(--ink);
    font-family: 'Inter', sans-serif;
    font-size: 15px;
    line-height: 1.7;
  }

  /* CAPA */
  .capa {
    min-height: 100vh;
    background: var(--deep);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 60px 40px;
    position: relative;
    overflow: hidden;
  }

  .capa::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(ellipse at 50% 60%, rgba(196,154,46,0.08) 0%, transparent 70%);
  }

  .capa-epigraph {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 1.05rem;
    color: var(--gold-light);
    opacity: 0.8;
    letter-spacing: 0.08em;
    margin-bottom: 48px;
  }

  .capa-nome {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(1rem, 3vw, 1.2rem);
    color: var(--gold);
    letter-spacing: 0.35em;
    text-transform: uppercase;
    margin-bottom: 16px;
  }

  .capa-titulo {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 600;
    font-size: clamp(2.8rem, 8vw, 5.5rem);
    color: #fff;
    line-height: 1.05;
    margin-bottom: 24px;
    letter-spacing: -0.01em;
  }

  .capa-titulo span {
    color: var(--gold);
  }

  .capa-subtitulo {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 1.35rem;
    color: rgba(255,255,255,0.6);
    margin-bottom: 56px;
    max-width: 600px;
  }

  .capa-frankl {
    border-top: 1px solid var(--line);
    border-bottom: 1px solid var(--line);
    padding: 28px 40px;
    max-width: 680px;
  }

  .capa-frankl blockquote {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 1.15rem;
    color: var(--gold-light);
    line-height: 1.6;
  }

  .capa-frankl cite {
    display: block;
    margin-top: 12px;
    font-family: 'Inter', sans-serif;
    font-size: 0.75rem;
    color: rgba(255,255,255,0.35);
    letter-spacing: 0.15em;
    text-transform: uppercase;
    font-style: normal;
  }

  .orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    opacity: 0.15;
    pointer-events: none;
  }
  .orb-1 { width: 400px; height: 400px; background: var(--gold); top: -100px; right: -100px; }
  .orb-2 { width: 300px; height: 300px; background: #4a90b8; bottom: -80px; left: -80px; }

  /* ESTRUTURA GERAL */
  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 0 32px;
  }

  /* SEPARADOR */
  .sep {
    display: flex;
    align-items: center;
    gap: 20px;
    margin: 64px 0 48px;
  }
  .sep-line { flex: 1; height: 1px; background: var(--line); }
  .sep-diamond {
    width: 8px; height: 8px;
    background: var(--gold);
    transform: rotate(45deg);
    flex-shrink: 0;
  }

  /* SEÇÕES */
  section { padding: 80px 0; }
  section:not(:last-child) { border-bottom: 1px solid var(--line); }

  .section-label {
    font-family: 'Inter', sans-serif;
    font-size: 0.68rem;
    font-weight: 600;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 12px;
  }

  .section-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(2rem, 5vw, 3rem);
    font-weight: 600;
    color: var(--deep);
    line-height: 1.15;
    margin-bottom: 32px;
  }

  .section-title em {
    font-style: italic;
    color: var(--rust);
  }

  .lead {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.3rem;
    color: var(--ink);
    line-height: 1.7;
    margin-bottom: 28px;
    font-weight: 300;
  }

  p { margin-bottom: 16px; color: #3a3028; }

  /* FRANKL QUOTE */
  .frankl-box {
    border-left: 3px solid var(--gold);
    padding: 20px 28px;
    margin: 36px 0;
    background: rgba(196,154,46,0.05);
  }
  .frankl-box blockquote {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 1.2rem;
    color: var(--deep);
    line-height: 1.6;
  }
  .frankl-box cite {
    display: block;
    margin-top: 8px;
    font-size: 0.75rem;
    color: var(--gold);
    letter-spacing: 0.12em;
    text-transform: uppercase;
    font-style: normal;
  }

  /* PILARES */
  .pilares {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 24px;
    margin: 40px 0;
  }

  .pilar {
    background: white;
    border: 1px solid var(--line);
    padding: 32px 28px;
    position: relative;
    transition: box-shadow 0.2s;
  }
  .pilar:hover { box-shadow: 0 8px 32px rgba(30,45,64,0.08); }

  .pilar-num {
    font-family: 'Cormorant Garamond', serif;
    font-size: 3.5rem;
    font-weight: 300;
    color: var(--gold);
    opacity: 0.3;
    line-height: 1;
    margin-bottom: 8px;
  }
  .pilar-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.4rem;
    font-weight: 600;
    color: var(--deep);
    margin-bottom: 10px;
  }
  .pilar p { font-size: 0.9rem; margin: 0; }

  /* FASES TIMELINE */
  .timeline { margin: 40px 0; }

  .fase {
    display: grid;
    grid-template-columns: 140px 1fr;
    gap: 0 32px;
    margin-bottom: 48px;
    position: relative;
  }

  .fase::before {
    content: '';
    position: absolute;
    left: 139px;
    top: 32px;
    bottom: -48px;
    width: 1px;
    background: var(--line);
  }
  .fase:last-child::before { display: none; }

  .fase-header {
    text-align: right;
    padding-top: 4px;
  }

  .fase-periodo {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.05rem;
    font-weight: 600;
    color: var(--gold);
    display: block;
  }

  .fase-nome {
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: rgba(30,45,64,0.45);
    display: block;
    margin-top: 2px;
  }

  .fase-dot {
    position: absolute;
    left: 132px;
    top: 6px;
    width: 16px; height: 16px;
    border-radius: 50%;
    background: var(--gold);
    border: 3px solid var(--parchment);
    box-shadow: 0 0 0 1px var(--gold);
  }

  .fase-body {
    padding-left: 20px;
  }

  .fase-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.5rem;
    font-weight: 600;
    color: var(--deep);
    margin-bottom: 12px;
  }

  .task-list {
    list-style: none;
    margin: 12px 0;
  }
  .task-list li {
    padding: 6px 0 6px 22px;
    position: relative;
    font-size: 0.9rem;
    color: #3a3028;
    border-bottom: 1px solid rgba(196,154,46,0.1);
  }
  .task-list li:last-child { border-bottom: none; }
  .task-list li::before {
    content: '◆';
    position: absolute;
    left: 0;
    color: var(--gold);
    font-size: 0.5rem;
    top: 10px;
  }

  /* FINANCEIRO */
  .financeiro-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin: 32px 0;
  }

  .fin-card {
    background: var(--deep);
    color: white;
    padding: 28px 24px;
    text-align: center;
  }

  .fin-valor {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2rem;
    font-weight: 600;
    color: var(--gold);
    display: block;
    margin-bottom: 4px;
  }

  .fin-label {
    font-size: 0.72rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    opacity: 0.6;
    display: block;
  }

  .fin-desc {
    font-size: 0.82rem;
    margin-top: 10px;
    opacity: 0.75;
    line-height: 1.5;
  }

  /* URGENTE */
  .urgente-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 20px;
    margin: 32px 0;
  }

  .urgente-card {
    border: 1px solid var(--gold);
    padding: 28px 24px;
    position: relative;
    background: white;
  }

  .urgente-tag {
    position: absolute;
    top: -10px;
    left: 20px;
    background: var(--gold);
    color: white;
    font-size: 0.65rem;
    font-weight: 600;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    padding: 3px 10px;
  }

  .urgente-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.3rem;
    font-weight: 600;
    color: var(--deep);
    margin-bottom: 10px;
  }

  .urgente-card p { font-size: 0.88rem; margin-bottom: 8px; }

  .urgente-valor {
    display: inline-block;
    margin-top: 10px;
    background: var(--deep);
    color: var(--gold);
    padding: 5px 14px;
    font-size: 0.85rem;
    font-weight: 600;
    font-family: 'Cormorant Garamond', serif;
  }

  /* TERAPEUTICO */
  .terapia-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 20px;
    margin: 32px 0;
  }

  .terapia-card {
    background: white;
    border: 1px solid var(--line);
    padding: 28px 24px;
    transition: border-color 0.2s;
  }
  .terapia-card:hover { border-color: var(--gold); }

  .terapia-icon {
    font-size: 1.6rem;
    margin-bottom: 12px;
    display: block;
  }

  .terapia-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.2rem;
    font-weight: 600;
    color: var(--deep);
    margin-bottom: 8px;
  }

  .terapia-card p { font-size: 0.85rem; }

  /* ELENA */
  .elena-box {
    background: linear-gradient(135deg, #f7f3ec 0%, #fdf8f0 100%);
    border: 1px solid rgba(196,154,46,0.3);
    padding: 40px;
    margin: 32px 0;
    position: relative;
  }
  .elena-box::before {
    content: '♡';
    position: absolute;
    top: 20px;
    right: 28px;
    font-size: 1.5rem;
    color: var(--gold);
    opacity: 0.4;
  }
  .elena-box h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.5rem;
    color: var(--rust);
    margin-bottom: 16px;
  }

  /* VALENCIA */
  .valencia-box {
    background: var(--deep);
    color: white;
    padding: 48px 40px;
    margin: 32px 0;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .valencia-box::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(ellipse at 50% 100%, rgba(196,154,46,0.12) 0%, transparent 70%);
  }
  .valencia-box h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2rem;
    color: var(--gold);
    margin-bottom: 8px;
    position: relative;
  }
  .valencia-box p {
    color: rgba(255,255,255,0.7);
    position: relative;
  }
  .valencia-meta {
    display: flex;
    justify-content: center;
    gap: 40px;
    margin: 28px 0;
    flex-wrap: wrap;
    position: relative;
  }
  .vmeta { text-align: center; }
  .vmeta-val {
    display: block;
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.8rem;
    color: var(--gold);
    font-weight: 600;
  }
  .vmeta-key {
    font-size: 0.7rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.45);
  }

  /* VERIFICAÇÃO */
  .check-table {
    width: 100%;
    border-collapse: collapse;
    margin: 28px 0;
  }
  .check-table th {
    text-align: left;
    font-size: 0.7rem;
    font-weight: 600;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--gold);
    padding: 10px 16px;
    border-bottom: 2px solid var(--gold);
  }
  .check-table td {
    padding: 12px 16px;
    font-size: 0.88rem;
    border-bottom: 1px solid var(--line);
    vertical-align: top;
  }
  .check-table tr:last-child td { border-bottom: none; }
  .check-table tr:hover td { background: rgba(196,154,46,0.03); }
  .badge {
    display: inline-block;
    padding: 2px 10px;
    font-size: 0.68rem;
    font-weight: 600;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    border-radius: 2px;
  }
  .badge-hoje { background: var(--rust); color: white; }
  .badge-semana { background: var(--deep); color: var(--gold); }
  .badge-mes { background: var(--sage); color: white; }
  .badge-trimestre { background: rgba(196,154,46,0.15); color: var(--gold); }

  /* CODA */
  .coda {
    background: var(--deep);
    color: white;
    padding: 80px 40px;
    text-align: center;
  }
  .coda blockquote {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: clamp(1.4rem, 4vw, 2.2rem);
    color: var(--gold-light);
    max-width: 700px;
    margin: 0 auto 24px;
    line-height: 1.5;
  }
  .coda-sub {
    font-size: 0.8rem;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: rgba(255,255,255,0.3);
  }
  .coda-assinatura {
    margin-top: 48px;
    font-family: 'Cormorant Garamond', serif;
    font-size: 1rem;
    color: rgba(255,255,255,0.35);
    letter-spacing: 0.1em;
  }

  @media (max-width: 640px) {
    .fase { grid-template-columns: 1fr; }
    .fase-header { text-align: left; }
    .fase::before { display: none; }
    .fase-dot { display: none; }
    .fase-body { padding-left: 0; }
    .container { padding: 0 20px; }
  }
</style>
</head>
<body>

<!-- CAPA -->
<div class="capa">
  <div class="orb orb-1"></div>
  <div class="orb orb-2"></div>

  <p class="capa-epigraph">Discretamente, pelo objetivo. Sem alarde, com atos.</p>
  <p class="capa-nome">Daniel — VISUALCAMPO · Raíces del Amor</p>
  <h1 class="capa-titulo">Plano<br><span>Grandioso</span></h1>
  <p class="capa-subtitulo">Da oficina em Ribeirão Preto às Fallas de Valencia — um plano de trabalho, sentido e amor</p>

  <div class="capa-frankl">
    <blockquote>
      "A vida nunca deixa de ter sentido — e isso inclui o sofrimento, a luta e a morte.<br>
      O que importa não é o que esperamos da vida, mas o que a vida espera de nós."
    </blockquote>
    <cite>— Viktor E. Frankl · Em Busca de Sentido</cite>
  </div>
</div>

<!-- SEÇÃO 1: FUNDAMENTO -->
<section style="background: white;">
  <div class="container">
    <div class="section-label">Fundamento · Por que fazer</div>
    <h2 class="section-title">A <em>missão</em> que dá sentido<br>a cada ato</h2>

    <p class="lead">Frankl chamava de "logoterapia" a cura pelo sentido. Você já tem o sentido: sua técnica de 25 anos, Elena, o cuidado com quem enxerga, a cura que você oferece. O que falta é organização desse potencial em fluxo de caixa e visibilidade.</p>

    <div class="frankl-box">
      <blockquote>"O ser humano capaz de encontrar um propósito pode suportar quase qualquer 'como'. A questão não é o que você tem — é para o que você usa o que tem."</blockquote>
      <cite>— Adaptação de Frankl ao seu contexto</cite>
    </div>

    <p>Você dispõe de dois negócios complementares, certificações terapêuticas sólidas, 25 anos de expertise técnica única no Brasil, relacionamentos de alto valor com médicos e clínicas, e — o mais raro — a coragem de começar hoje.</p>

    <div class="pilares">
      <div class="pilar">
        <div class="pilar-num">I</div>
        <div class="pilar-title">Técnica Clínica</div>
        <p>VISUALCAMPO — perimetria, lensometria, manutenção de equipamentos oftalmológicos. Expertise intransferível, mercado restrito, margens altas.</p>
      </div>
      <div class="pilar">
        <div class="pilar-num">II</div>
        <div class="pilar-title">Cuidado Terapêutico</div>
        <p>Raíces del Amor — Reiki, Constelação Familiar, Reflexologia, OH Cards. Elena e Daniel: uma dupla de complementaridade rara.</p>
      </div>
      <div class="pilar">
        <div class="pilar-num">III</div>
        <div class="pilar-title">Visibilidade Local</div>
        <p>Ribeirão Preto precisa conhecer o que você já é. A cidade ainda não sabe o que tem em seu centro.</p>
      </div>
      <div class="pilar">
        <div class="pilar-num">IV</div>
        <div class="pilar-title">Destino: Valencia</div>
        <p>A viagem com Elena não é luxo — é o horizonte que move tudo. A meta concreta que transforma plano em motor.</p>
      </div>
    </div>
  </div>
</section>

<!-- SEÇÃO 2: URGENTE AGORA -->
<section>
  <div class="container">
    <div class="section-label">Prioridade Imediata · Esta semana</div>
    <h2 class="section-title">O que você faz<br><em>hoje e amanhã</em></h2>

    <p class="lead">Três oportunidades reais já na sua frente. Estas são ações com retorno financeiro imediato. Nenhuma exige investimento — apenas técnica, que você já tem.</p>

    <div class="urgente-cards">

      <div class="urgente-card">
        <span class="urgente-tag">Hoje</span>
        <div class="urgente-title">Lensômetro Manual + Lâmpada de Fenda</div>
        <p><strong>Estado:</strong> necessitam restauração e revisão.</p>
        <p><strong>Ação:</strong> Elabore orçamento detalhado com três valores — econômico, padrão e premium (com garantia estendida). Apresente ao cliente descrevendo tecnicamente o que será feito, usando linguagem CNV: "o que precisa ser restaurado é..." sem depreciar o equipamento.</p>
        <p><strong>Posicionamento Tesla:</strong> "Estes são instrumentos de precisão. O cuidado que recebem define a qualidade do diagnóstico do seu paciente."</p>
        <span class="urgente-valor">Estimativa: R$ 800 – R$ 2.400</span>
      </div>

      <div class="urgente-card">
        <span class="urgente-tag">Esta semana</span>
        <div class="urgente-title">Instalação Elétrica — Dr. Benoni</div>
        <p><strong>Estado:</strong> falha elétrica na sala de exames.</p>
        <p><strong>Ação:</strong> Visita técnica diagnóstica (cobrada separadamente). Mapeie o circuito, identifique a origem da falha. Entregue laudo técnico escrito — isso gera confiança e justifica o valor do serviço.</p>
        <p><strong>Diferencial:</strong> Você conhece o impacto de ruído elétrico em equipamentos de diagnóstico. Use isso: "Uma instalação inadequada compromete a calibração dos seus equipamentos."</p>
        <span class="urgente-valor">Visita diagnóstica: R$ 350 – R$ 600</span>
      </div>

      <div class="urgente-card">
        <span class="urgente-tag">Esta semana</span>
        <div class="urgente-title">Visibilidade em Ribeirão Preto</div>
        <p><strong>Ação imediata:</strong> Atualize o Google Meu Negócio de VISUALCAMPO com fotos reais, horário e descrição precisa. Faça o mesmo para Raíces del Amor.</p>
        <p><strong>WhatsApp:</strong> Envie mensagem personalizada (CNV + Carnegie) para 5 médicos ou clínicas que você já atendeu, perguntando como os equipamentos estão — sem vender, apenas cuidando.</p>
        <p><strong>Resultado esperado:</strong> Pelo menos 1 retorno com demanda em 7 dias.</p>
        <span class="urgente-valor">Investimento: zero. ROI: alto.</span>
      </div>

    </div>
  </div>
</section>

<!-- SEÇÃO 3: PLANO FINANCEIRO -->
<section style="background: white;">
  <div class="container">
    <div class="section-label">Mapa Financeiro · Metas por fase</div>
    <h2 class="section-title">Quanto, de onde<br>e <em>quando</em></h2>

    <p class="lead">A viagem a Valencia em março de 2027 exige organização de recursos ao longo de 18 meses. O plano abaixo é conservador e realista, baseado nos seus dois negócios.</p>

    <div class="financeiro-grid">
      <div class="fin-card">
        <span class="fin-valor">R$ 3.500</span>
        <span class="fin-label">Meta mensal mínima</span>
        <p class="fin-desc">VISUALCAMPO: 2 atendimentos técnicos + 1 contrato de manutenção preventiva</p>
      </div>
      <div class="fin-card">
        <span class="fin-valor">R$ 1.800</span>
        <span class="fin-label">Meta mensal Raíces</span>
        <p class="fin-desc">12 sessões terapêuticas mensais × R$ 150 (escalonável com Elena)</p>
      </div>
      <div class="fin-card">
        <span class="fin-valor">R$ 800</span>
        <span class="fin-label">Reserva mensal viagem</span>
        <p class="fin-desc">Separado automaticamente todo mês em conta específica para Valencia</p>
      </div>
      <div class="fin-card">
        <span class="fin-valor">R$ 14.400</span>
        <span class="fin-label">Fundo em 18 meses</span>
        <p class="fin-desc">Suficiente para voos + hotel + vivência por 10–12 dias em Valencia na temporada Fallas</p>
      </div>
    </div>

    <div class="frankl-box">
      <blockquote>"Não pergunte o que a vida pode te dar. Pergunte o que você pode dar à vida — e o retorno virá como consequência natural de quem você se torna no processo."</blockquote>
      <cite>— Aplicação Frankl ao planejamento financeiro</cite>
    </div>

  </div>
</section>

<!-- SEÇÃO 4: TIMELINE -->
<section>
  <div class="container">
    <div class="section-label">Cronograma · Fase a fase</div>
    <h2 class="section-title">O caminho<br><em>mês a mês</em></h2>

    <div class="timeline">

      <div class="fase">
        <div class="fase-header">
          <span class="fase-periodo">Ago–Set 2025</span>
          <span class="fase-nome">Fase 1</span>
        </div>
        <div class="fase-dot"></div>
        <div class="fase-body">
          <div class="fase-title">Ignição — Organizar o que já existe</div>
          <ul class="task-list">
            <li>Executar os 3 trabalhos urgentes (lensômetro, lâmpada de fenda, Dr. Benoni)</li>
            <li>Atualizar Google Meu Negócio para ambas as marcas</li>
            <li>Criar lista dos 20 contatos médicos mais quentes — ativar 5 por semana via WhatsApp CNV</li>
            <li>Definir com Elena o calendário fixo de sessões terapêuticas (terças + uma tarde extra)</li>
            <li>Abrir conta separada "Fundo Valencia" — depósito inicial simbólico de qualquer valor</li>
            <li>Registrar receitas e despesas em planilha simples semanal</li>
          </ul>
        </div>
      </div>

      <div class="fase">
        <div class="fase-header">
          <span class="fase-periodo">Out–Nov 2025</span>
          <span class="fase-nome">Fase 2</span>
        </div>
        <div class="fase-dot"></div>
        <div class="fase-body">
          <div class="fase-title">Consolidação — Criar fluxo recorrente</div>
          <ul class="task-list">
            <li>Fechar pelo menos 2 contratos de manutenção preventiva mensal com clínicas (R$ 400–800/mês cada)</li>
            <li>Lançar formalmente as sessões de OH Cards como serviço específico (grupo ou individual)</li>
            <li>Realizar 1 evento de Constelação Familiar com 6–10 participantes (R$ 200–350/pessoa)</li>
            <li>Postar semanalmente no Instagram: VISUALCAMPO (técnico/educativo) e Raíces (terapêutico/poético)</li>
            <li>Produzir 1 vídeo curto mostrando um equipamento restaurado — prova social concreta</li>
          </ul>
        </div>
      </div>

      <div class="fase">
        <div class="fase-header">
          <span class="fase-periodo">Dez 2025 – Fev 2026</span>
          <span class="fase-nome">Fase 3</span>
        </div>
        <div class="fase-dot"></div>
        <div class="fase-body">
          <div class="fase-title">Expansão — Novos produtos e alcance</div>
          <ul class="task-list">
            <li>Lançar o curso digital no Kiwify: "Restauração do Zeiss Stratus OCT 3000" (ou módulo introdutório)</li>
            <li>Criar pacote "Elena + Daniel": sessão combinada Reiki + Constelação + Reflexologia (sessão de casal)</li>
            <li>Prospectar clínicas no corredor Ribeirão–Franca–Jaú com abordagem SPIN personalizada</li>
            <li>Iniciar prática regular de Radiestesia como ferramenta complementar nas sessões (reativação da certificação)</li>
            <li>Avaliar renda acumulada: ajustar meta ou antecipar compra de passagens</li>
          </ul>
        </div>
      </div>

      <div class="fase">
        <div class="fase-header">
          <span class="fase-periodo">Mar–Dez 2026</span>
          <span class="fase-nome">Fase 4</span>
        </div>
        <div class="fase-dot"></div>
        <div class="fase-body">
          <div class="fase-title">Maturidade — Sistema funcionando</div>
          <ul class="task-list">
            <li>Manter 3–4 contratos de manutenção preventiva ativos = renda previsível</li>
            <li>Raíces del Amor com agenda de 60–80% de ocupação semanal</li>
            <li>Produto digital gerando renda passiva mínima de R$ 500/mês</li>
            <li>Comprar passagens para Valencia (melhor preço: 6–8 meses de antecedência)</li>
            <li>Reservar hotel em Valencia para 15–22 de março de 2027</li>
            <li>Elena com acompanhamento de saúde atualizado e bem-estar consolidado</li>
          </ul>
        </div>
      </div>

      <div class="fase">
        <div class="fase-header">
          <span class="fase-periodo">Jan–Mar 2027</span>
          <span class="fase-nome">Fase 5</span>
        </div>
        <div class="fase-dot"></div>
        <div class="fase-body">
          <div class="fase-title">Colheita — Partida para Valencia</div>
          <ul class="task-list">
            <li>Preparar negócio para 2 semanas sem atendimento presencial (agendamento antecipado)</li>
            <li>Documentar aprendizados da viagem para conteúdo posterior</li>
            <li>Viver as Fallas com Elena plenamente — fruição total do que foi construído</li>
            <li>Retornar com energia renovada e horizonte ampliado para o próximo ciclo</li>
          </ul>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- SEÇÃO 5: RECURSOS TERAPÊUTICOS -->
<section style="background: white;">
  <div class="container">
    <div class="section-label">Seus recursos · O que você já tem</div>
    <h2 class="section-title">Seu arsenal<br><em>terapêutico</em></h2>

    <p class="lead">Você não está começando do zero. Você está ativando o que já existe. Cada certificação é um serviço que pode ser oferecido ainda esta semana.</p>

    <div class="terapia-grid">
      <div class="terapia-card">
        <span class="terapia-icon">✦</span>
        <div class="terapia-title">Reiki Nível Master<br>(Usui + Gendai)</div>
        <p>Serviço: sessões individuais R$ 120–200. Potencial imediato: retomar as terças com 3–4 clientes/semana. Ofereça "pacote mensal" de 4 sessões com desconto fidelidade.</p>
      </div>
      <div class="terapia-card">
        <span class="terapia-icon">◈</span>
        <div class="terapia-title">Constelação Familiar</div>
        <p>Serviço de maior valor agregado. Evento presencial com 8–12 pessoas: R$ 250–400/pessoa. Faça 1 por mês = R$ 2.000–4.000 extras. Parceria com Elena potencializa.</p>
      </div>
      <div class="terapia-card">
        <span class="terapia-icon">◉</span>
        <div class="terapia-title">OH Cards — Especialista</div>
        <p>Diferencial raro: você tem formação direta com o criador. Use isso. Crie sessão específica "Cartas OH para autoconhecimento" — R$ 150–250. Grupo de 6: R$ 900+.</p>
      </div>
      <div class="terapia-card">
        <span class="terapia-icon">✿</span>
        <div class="terapia-title">Reflexologia Podal</div>
        <p>Sessão de 50min: R$ 100–150. Combine com Reiki em "sessão integrativa" — serviço diferenciado que justifica R$ 200+. Elena pode incorporar em seu protocolo também.</p>
      </div>
      <div class="terapia-card">
        <span class="terapia-icon">◎</span>
        <div class="terapia-title">CNV — Comunicação<br>Não Violenta</div>
        <p>Não é um serviço isolado — é o fio que torna todos os outros mais eficazes. Aplique em cada proposta técnica, cada sessão, cada mensagem de WhatsApp. É seu maior ativo invisível.</p>
      </div>
      <div class="terapia-card">
        <span class="terapia-icon">⟁</span>
        <div class="terapia-title">Radiestesia</div>
        <p>Reative com prática semanal pessoal por 30 dias. Não ofereça como serviço ainda — mas incorpore como ferramenta de discernimento pessoal e intuição clínica. O momento de monetizar virá.</p>
      </div>
    </div>
  </div>
</section>

<!-- SEÇÃO 6: ELENA -->
<section>
  <div class="container">
    <div class="section-label">Elena · O centro de tudo</div>
    <h2 class="section-title">Cuidar de quem<br><em>cuida ao seu lado</em></h2>

    <div class="elena-box">
      <h3>Harmonizar as questões físicas de Elena</h3>
      <p>Elena é sua companheira de vida e de missão. Sua saúde é parte do plano — não apenas como amor, mas como co-criadora de Raíces del Amor. Sem ela plena, o projeto não é completo.</p>

      <ul class="task-list" style="margin-top: 16px;">
        <li><strong>Esta semana:</strong> Identificar com ela quais são as questões físicas prioritárias e agendar consulta médica específica. Nomeie o problema para poder tratá-lo.</li>
        <li><strong>Tratamento integrado:</strong> Você mesmo pode oferecer sessões regulares de Reiki e Reflexologia para Elena — cuidado prático e íntimo, não apenas simbólico.</li>
        <li><strong>Rotina de bem-estar:</strong> Definir juntos uma rotina semanal mínima: movimento (caminhada), alimentação consciente, e um momento de silêncio compartilhado.</li>
        <li><strong>Participação no projeto:</strong> Que Elena saiba que Valencia não é uma meta sua — é a meta de vocês dois. Isso multiplica a força motivacional de cada ação.</li>
        <li><strong>Constelação Familiar:</strong> Considere realizar uma constelação focada na saúde de Elena, conduzida por um par de confiança ou em workshop com outros consteladores.</li>
      </ul>
    </div>

    <div class="frankl-box">
      <blockquote>"O amor é a única maneira de apreender outro ser humano na mais profunda essência de sua personalidade. Amar é ver o potencial do amado e ajudá-lo a realizá-lo."</blockquote>
      <cite>— Viktor E. Frankl</cite>
    </div>
  </div>
</section>

<!-- SEÇÃO 7: VERIFICAÇÃO -->
<section style="background: white;">
  <div class="container">
    <div class="section-label">Verificação · Noção de evolução</div>
    <h2 class="section-title">Como saber<br>que está <em>funcionando</em></h2>

    <p>Frankl ensinava que a vida precisa ser mensurável em sentido — não apenas em números. Aqui, você mede ambos.</p>

    <table class="check-table">
      <thead>
        <tr>
          <th>Prazo</th>
          <th>Ação</th>
          <th>Indicador de sucesso</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><span class="badge badge-hoje">Hoje</span></td>
          <td>Emitir orçamento lensômetro + lâmpada de fenda</td>
          <td>Orçamento enviado ao cliente</td>
        </tr>
        <tr>
          <td><span class="badge badge-hoje">Hoje</span></td>
          <td>Agendar visita técnica Dr. Benoni</td>
          <td>Data confirmada via WhatsApp</td>
        </tr>
        <tr>
          <td><span class="badge badge-semana">Semana 1</span></td>
          <td>Atualizar Google Meu Negócio (ambas marcas)</td>
          <td>Perfis completos e visíveis</td>
        </tr>
        <tr>
          <td><span class="badge badge-semana">Semana 1</span></td>
          <td>Contatar 5 médicos com mensagem CNV</td>
          <td>5 mensagens enviadas, aguardar retorno</td>
        </tr>
        <tr>
          <td><span class="badge badge-semana">Semana 2</span></td>
          <td>Agenda de Elena organizada (sessões terapêuticas)</td>
          <td>Calendário compartilhado definido</td>
        </tr>
        <tr>
          <td><span class="badge badge-mes">Mês 1</span></td>
          <td>Primeiro depósito no Fundo Valencia</td>
          <td>Qualquer valor — o ato importa mais</td>
        </tr>
        <tr>
          <td><span class="badge badge-mes">Mês 1</span></td>
          <td>Receita bruta mínima</td>
          <td>R$ 2.000 (conservador) a R$ 4.000 (meta)</td>
        </tr>
        <tr>
          <td><span class="badge badge-trimestre">Trimestre 1</span></td>
          <td>Contratos preventivos firmados</td>
          <td>Mínimo 2 clínicas com contrato mensal</td>
        </tr>
        <tr>
          <td><span class="badge badge-trimestre">Trimestre 1</span></td>
          <td>1 evento de Constelação Familiar realizado</td>
          <td>Realizado, feedbacks coletados</td>
        </tr>
        <tr>
          <td><span class="badge badge-trimestre">Trimestre 2</span></td>
          <td>Fundo Valencia</td>
          <td>R$ 4.000+ acumulados</td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

<!-- SEÇÃO 8: VALENCIA -->
<section>
  <div class="container">
    <div class="section-label">O Destino · Março 2027</div>
    <h2 class="section-title">Valencia<br><em>com Elena</em></h2>

    <div class="valencia-box">
      <h3>Las Fallas de Valencia — 15 a 19 de Março de 2027</h3>
      <p>Não é um prêmio distante. É o ponto fixo no horizonte que orienta cada ação de hoje.</p>

      <div class="valencia-meta">
        <div class="vmeta">
          <span class="vmeta-val">19 Mar</span>
          <span class="vmeta-key">La Cremà</span>
        </div>
        <div class="vmeta">
          <span class="vmeta-val">~18 meses</span>
          <span class="vmeta-key">De hoje até lá</span>
        </div>
        <div class="vmeta">
          <span class="vmeta-val">R$ 800/mês</span>
          <span class="vmeta-key">Reserva mensal</span>
        </div>
        <div class="vmeta">
          <span class="vmeta-val">2 pessoas</span>
          <span class="vmeta-key">Daniel + Elena</span>
        </div>
      </div>

      <p style="color: rgba(255,255,255,0.5); font-size: 0.85rem;">Aquela figura de Arlequim que você viu — vocês vão estar na praça, de frente para ela, antes que ela seja consumida pelo fogo. Esse é o objetivo.</p>
    </div>
  </div>
</section>

<!-- CODA -->
<div class="coda">
  <blockquote>
    "O exemplo são seus atos."<br>
    <em style="font-size: 0.75em; opacity: 0.7;">— Renê Mey</em>
  </blockquote>

  <p class="coda-sub">Discretamente. Pelo objetivo. Sem alarde.</p>

  <div style="margin: 48px auto; width: 40px; height: 1px; background: rgba(196,154,46,0.4);"></div>

  <p style="color: rgba(255,255,255,0.35); font-size: 0.9rem; font-family: 'Cormorant Garamond', serif; font-style: italic; max-width: 500px; margin: 0 auto 16px;">
    Que seja grande.<br>
    Que seja abençoado por Deus.<br>
    Peço humildemente a permissão de ser total.
  </p>

  <p class="coda-assinatura">DANIEL · VISUALCAMPO · RAÍCES DEL AMOR · 2025–2027</p>
</div>

</body>
</html>

