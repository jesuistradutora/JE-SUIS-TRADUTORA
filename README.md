# JE-SUIS-TRADUTORA
JE SUIS TRADUTORA WEBSITE
<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>JE SUIS TRADUTORA — Agência de Tradução</title>
  <meta name="description" content="JE SUIS TRADUTORA: Tradução, versão, revisão, transcrição, legendagem, interpretação e criação de roteiros. Cobrança por projeto. PT • EN • FR • ES." />
  <style>
    :root{
      --primary:#4D41E2; /* roxo */
      --accent:#F4C500;  /* amarelo */
      --mint:#C4F5D4;    /* verde menta */
      --orange:#F29B3E;  /* laranja */
      --ink:#0f172a;     /* slate-900 */
      --text:#334155;    /* slate-700 */
      --muted:#64748b;   /* slate-500 */
      --bg:#f8fafc;      /* slate-50 */
      --card:#ffffff;
    }
    /* Tipografias: placeholders — quando tiver os arquivos das fontes, basta declarar @font-face com esses nomes */
    body{font-family: system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,"Helvetica Neue",Arial,"Noto Color Emoji","Apple Color Emoji",sans-serif; color:var(--text); background:linear-gradient(180deg,#fff 0,var(--bg) 100%); margin:0}
    .brand{font-family:"Pleasewritemeasong","Letters for Learners",inherit}
    .wrap{max-width:1100px;margin:0 auto;padding:0 20px}
    header{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.8);backdrop-filter:saturate(1.2) blur(8px);border-bottom:1px solid #e2e8f0}
    nav a{color:#0f172a;text-decoration:none;margin:0 10px;font-size:14px}
    nav a:hover{text-decoration:underline}
    .btn{display:inline-flex;align-items:center;gap:.5rem;border-radius:14px;padding:.8rem 1rem;border:1px solid #e2e8f0;background:#fff;color:#0f172a;text-decoration:none;font-weight:600}
    .btn.primary{background:var(--ink);color:#fff;border-color:var(--ink)}
    .btn.whatsapp{position:fixed;right:20px;bottom:20px;background:#fff;border-color:#e2e8f0;box-shadow:0 8px 24px rgba(2,6,23,.1)}
    .hero{padding:64px 0 48px;display:grid;grid-template-columns:1.2fr .8fr;gap:32px}
    @media (max-width:900px){.hero{grid-template-columns:1fr}} 
    h1{font-size:42px;line-height:1.1;color:#0f172a;margin:0}
    h2{font-size:28px;color:#0f172a;margin:0}
    .muted{color:var(--muted)}
    .badge{display:inline-block;padding:.35rem .7rem;border-radius:999px;font-size:12px;border:1px solid #e2e8f0;background:#fff}
    .cards{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    @media (max-width:900px){.cards{grid-template-columns:1fr 1fr}} 
    @media (max-width:640px){.cards{grid-template-columns:1fr}} 
    .card{background:var(--card);border:1px solid #e2e8f0;border-radius:20px;padding:18px}
    .pill{display:inline-block;border:1px solid #e2e8f0;border-radius:999px;padding:8px 12px;background:#fff;font-size:14px;margin:6px 6px 0 0}
    section{padding:54px 0}
    .cta{border-radius:24px;padding:28px;background:var(--ink);color:#fff;display:flex;flex-wrap:wrap;align-items:center;gap:16px}
    footer{padding:32px 0;color:var(--muted)}
    .grid-2{display:grid;grid-template-columns:1fr 1fr;gap:24px}
    @media (max-width:900px){.grid-2{grid-template-columns:1fr}}
    .logo-placeholder{width:100%;aspect-ratio:4/3;border-radius:22px;background:linear-gradient(135deg,var(--mint),#e5e7eb 60%);display:flex;align-items:end;justify-content:flex-start;padding:16px;font-weight:600;color:#0f172a}
    .chip{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border-radius:999px;background:#fff;border:1px solid #e2e8f0;font-size:13px}
    .step{display:flex;gap:12px;align-items:flex-start}
    .step .num{width:28px;height:28px;border-radius:50%;border:1px solid #cbd5e1;display:flex;align-items:center;justify-content:center;font-weight:700;color:#0f172a}
    .portfolio-item{padding:14px 16px;border:1px solid #e2e8f0;border-radius:14px;background:#fff}
    .i18n-select{border:1px solid #e2e8f0;background:#fff;border-radius:10px;padding:8px}
    .hl{color:var(--primary)}
    .accent{color:var(--orange)}
    a{color:var(--primary)} a:hover{text-decoration:underline}
  </style>
</head>
<body>
  <header>
    <div class="wrap" style="display:flex;align-items:center;justify-content:space-between;padding:12px 0;gap:16px">
      <a href="#home" class="brand" style="display:flex;align-items:center;gap:10px;text-decoration:none;color:#0f172a">
        <span style="display:inline-grid;place-items:center;width:36px;height:36px;border-radius:10px;background:var(--primary);color:#fff;font-weight:800">JT</span>
        <strong>JE SUIS TRADUTORA</strong>
      </a>
      <nav style="display:flex;align-items:center;gap:8px">
        <a href="#servicos" data-i18n="nav.services">Serviços</a>
        <a href="#portfolio" data-i18n="nav.portfolio">Portfólio</a>
        <a href="#sobre" data-i18n="nav.about">Sobre</a>
        <a href="#contato" data-i18n="nav.contact">Contato</a>
        <select id="lang" class="i18n-select" aria-label="Idioma">
          <option value="pt">PT</option>
          <option value="en">EN</option>
          <option value="fr">FR</option>
          <option value="es">ES</option>
        </select>
        <a href="#contato" class="btn primary" data-i18n="nav.cta">Pedir orçamento</a>
      </nav>
    </div>
  </header>

  <main id="home" class="wrap">
    <!-- HERO -->
    <section class="hero">
      <div>
        <h1 class="brand" data-i18n="hero.title">JE SUIS TRADUTORA</h1>
        <p class="muted" style="font-size:18px;margin:12px 0 18px" data-i18n="hero.tag">Tradução profissional para quem precisa de precisão e potência poética.</p>
        <div style="display:flex;gap:10px;flex-wrap:wrap">
          <a class="btn primary" href="#contato" data-i18n="hero.btn1">Fale com a gente</a>
          <span class="chip">PT • EN • FR • ES</span>
          <span class="chip" title="Cobrança por projeto" data-i18n="hero.badge">Cobrança por projeto</span>
        </div>
        <p style="margin-top:14px;font-size:14px" class="muted">ID visual: <span class="hl">#4D41E2</span> · <span class="hl" style="color:var(--accent)">#F4C500</span> · <span class="hl" style="color:var(--mint)">#C4F5D4</span> · <span class="hl" style="color:var(--orange)">#F29B3E</span></p>
      </div>
      <div class="logo-placeholder">Substitua por sua logomarca quando enviar</div>
    </section>

    <!-- SERVIÇOS -->
    <section id="servicos">
      <h2 data-i18n="services.title">Serviços</h2>
      <p class="muted" style="margin:6px 0 18px" data-i18n="services.desc">Soluções sob medida em linguagem, presença e contexto.</p>
      <div class="cards">
        <div class="card"><strong data-i18n="services.items.revisao">Revisão</strong><p class="muted" data-i18n="services.items.revisaoD">Aprimoramos estilo, gramática e consistência terminológica.</p></div>
        <div class="card"><strong data-i18n="services.items.traducao">Tradução</strong><p class="muted" data-i18n="services.items.traducaoD">PT↔EN↔FR↔ES, com precisão e sensibilidade cultural.</p></div>
        <div class="card"><strong data-i18n="services.items.versao">Versão</strong><p class="muted" data-i18n="services.items.versaoD">Adaptamos do português para outros idiomas mantendo voz autoral.</p></div>
        <div class="card"><strong data-i18n="services.items.transcricao">Transcrição</strong><p class="muted" data-i18n="services.items.transcricaoD">Registro fiel de áudios e vídeos, com tratamento de falas.</p></div>
        <div class="card"><strong data-i18n="services.items.legendagem">Legendagem</strong><p class="muted" data-i18n="services.items.legendagemD">Tradução e revisão de legendas com timing e normas.</p></div>
        <div class="card"><strong data-i18n="services.items.simultanea">Tradução simultânea</strong><p class="muted" data-i18n="services.items.simultaneaD">Interpretação em tempo real para eventos e reuniões.</p></div>
        <div class="card"><strong data-i18n="services.items.consecutiva">Tradução consecutiva</strong><p class="muted" data-i18n="services.items.consecutivaD">Interpretação com pausas para ambientes técnicos.</p></div>
        <div class="card"><strong data-i18n="services.items.roteiro">Criação de roteiro</strong><p class="muted" data-i18n="services.items.roteiroD">Dramaturgia, audiovisual, publicidade, eventos e mais.</p></div>
      </div>
      <div style="margin-top:12px">
        <span class="pill">PT • EN • FR • ES — <span data-i18n="services.pairs">todas as combinações</span></span>
        <span class="pill" data-i18n="services.billing">Cobrança feita por projeto</span>
      </div>
    </section>

    <!-- PORTFÓLIO -->
    <section id="portfolio">
      <h2 data-i18n="portfolio.title">Principais traduções</h2>
      <p class="muted" style="margin:6px 0 18px" data-i18n="portfolio.desc">Uma amostra de trabalhos em cultura, mercado e tecnologia.</p>
      <div class="cards">
        <div class="portfolio-item"><strong>Google</strong><br><span class="muted" data-i18n="portfolio.google">Versão pt→en de estudos e pesquisas no Brasil: “Afroempreendedorismo”, “Inteligência Artificial” e “Escassez de profissionais de tecnologia”. (2022)</span></div>
        <div class="portfolio-item"><strong>TED Talks</strong><br><span class="muted" data-i18n="portfolio.ted">Revisão de legendas em pt e versão pt→en de palestras sobre sustentabilidade, cultura popular e storytelling. (2021–2022)</span></div>
        <div class="portfolio-item"><strong>WhatsApp</strong><br><span class="muted" data-i18n="portfolio.whatsapp">Versão pt→en de campanhas de lançamento, planejamento de RP e mídia do WhatsApp Brasil. (2022)</span></div>
        <div class="portfolio-item"><strong>Tiger Beer</strong><br><span class="muted" data-i18n="portfolio.tiger">Versão pt→en de campanhas de lançamento de produtos e eventos. (2022)</span></div>
        <div class="portfolio-item"><strong>Teatro Vila Velha</strong><br><span class="muted" data-i18n="portfolio.tvv">Versão pt→en de materiais de comunicação para parceiros internacionais. (2022)</span></div>
        <div class="portfolio-item"><strong>Ambev</strong><br><span class="muted" data-i18n="portfolio.ambev">Versão pt→en de roteiro da cerimônia de apresentação de novos sócios. (2023)</span></div>
        <div class="portfolio-item"><strong>“Doc HAI África”</strong><br><span class="muted" data-i18n="portfolio.hai">Transcrição e legendagem pt→en do documentário de Antônio Galvão. (2025)</span></div>
        <div class="portfolio-item"><strong>Produtora Errante — “Bóia”</strong><br><span class="muted" data-i18n="portfolio.boia">Transcrição e legendagem pt→en do longa de Luiz e Ricardo Pretti. (2025)</span></div>
        <div class="portfolio-item"><strong>“Paxukxay Nakyã”</strong><br><span class="muted" data-i18n="portfolio.pax">Transcrição e legendagem pt→en do documentário dirigido por Nino Franco. (2023)</span></div>
        <div class="portfolio-item"><strong>“Ana e Tadeu”</strong><br><span class="muted" data-i18n="portfolio.ana">Versão pt→en da dramaturgia de Mônica Santana. (2023)</span></div>
        <div class="portfolio-item"><strong>“Porto de Origem”</strong><br><span class="muted" data-i18n="portfolio.porto">Transcrição e legendagem pt→en + pt→es, doc. dirigido por Bernard Attal. (2022)</span></div>
        <div class="portfolio-item"><strong>Websérie “Por trás dos palcos” — Festival Farraial</strong><br><span class="muted" data-i18n="portfolio.farraial">Transcrição para a agência InHaus. (2022)</span></div>
        <div class="portfolio-item"><strong>“Catadoras de Luxo – Heroínas Invisíveis”</strong><br><span class="muted" data-i18n="portfolio.catadoras">Versão pt→en da obra documental. (2021)</span></div>
      </div>
    </section>

    <!-- SOBRE / BIO -->
    <section id="sobre" class="grid-2">
      <div>
        <h2 data-i18n="about.title">Sobre a agência</h2>
        <p style="margin-top:10px" data-i18n="about.text">A agência nasce do desejo de propor outro espectro na atividade de tradução. Superar limitações técnicas e abandonar a cultura solitária e mecânica. Passear por distintas expressões artísticas além da literatura e observar as alterações linguísticas quase como uma renovação celular vibrando em corpo vivo. Desconstruir gramáticas obsoletas e dar um zoom nas variações regionais, temporais e políticas. Quem está por trás da agência tem histórias fundidas com teatro, escrita, educação e produção cultural e até aqui, traduzimos informações com potencial de alteração da realidade rumo à expansão futurista.</p>
        <div style="margin-top:16px;display:grid;gap:10px">
          <div class="step"><div class="num">1</div><div><strong data-i18n="process.1t">Briefing vivo</strong><div class="muted" data-i18n="process.1d">Objetivo, público e referências culturais.</div></div></div>
          <div class="step"><div class="num">2</div><div><strong data-i18n="process.2t">Execução especializada</strong><div class="muted" data-i18n="process.2d">Profissional alinhado ao tema e glossários.</div></div></div>
          <div class="step"><div class="num">3</div><div><strong data-i18n="process.3t">Revisão dupla</strong><div class="muted" data-i18n="process.3d">Controle de qualidade e padronização.</div></div></div>
          <div class="step"><div class="num">4</div><div><strong data-i18n="process.4t">Entrega & pós</strong><div class="muted" data-i18n="process.4d">Ajustes finos e suporte após envio.</div></div></div>
        </div>
      </div>
      <div class="card">
        <h3 class="brand" style="margin:0">Rebeca Ribeiro Lima</h3>
        <p class="muted" style="margin:4px 0 10px">atriz • tradutora • cronista • roteirista</p>
        <p data-i18n="bio.text">Rebeca é atriz, tradutora, cronista e roteirista. Lançou “Cotidiano arde e o resto é silêncio” pela editora Urutau e encontra-se em fase de montagem do monólogo autoral “Sugar Baby do Brasil”, com o apoio do IBT e da Funarte. Estreou em 2024 no audiovisual no longa “Vila Buarque” (título em definição) de Luiz e Ricardo Pretti e no curta “Como vivem os mortos” da produtora É Nós na Fita. Traduziu a dramaturgia “Ana e Tadeu” de Mônica Santana e o longa “Porto de Origem” de Bernard Attal. Nos palcos desde 2003, atuou em mais de 20 espetáculos.</p>
      </div>
    </section>

    <!-- CTA -->
    <section>
      <div class="cta">
        <div style="flex:1;min-width:240px">
          <h2 class="brand" data-i18n="cta.title">Pronto(a) para o próximo projeto?</h2>
          <p class="muted" style="color:#e2e8f0" data-i18n="cta.desc">Envie arquivo, prazo e objetivo. Retornamos com o orçamento.</p>
        </div>
        <a class="btn" href="#contato" data-i18n="cta.btn">Solicitar orçamento</a>
      </div>
    </section>

    <!-- CONTATO -->
    <section id="contato" class="grid-2">
      <div>
        <h2 data-i18n="contact.title">Contato</h2>
        <p class="muted" style="margin:6px 0 16px" data-i18n="contact.desc">Atendimento seg–sex, 9h–18h (BRT).</p>
        <p><strong>E-mail:</strong> <a href="mailto:jesuistradutora@gmail.com">jesuistradutora@gmail.com</a></p>
        <p><strong>WhatsApp:</strong> <a href="https://wa.me/5571999061164" target="_blank" rel="noopener">+55 71 99906-1164</a></p>
        <p class="muted" data-i18n="contact.billing">Cobrança feita por projeto.</p>
      </div>
      <form class="card" action="mailto:jesuistradutora@gmail.com" method="post" enctype="text/plain">
        <label>Nome<br><input name="nome" required style="width:100%;padding:10px;border:1px solid #e2e8f0;border-radius:12px" /></label>
        <br><br>
        <label>E-mail<br><input type="email" name="email" required style="width:100%;padding:10px;border:1px solid #e2e8f0;border-radius:12px" /></label>
        <br><br>
        <label>Mensagem<br><textarea name="mensagem" required style="width:100%;min-height:120px;padding:10px;border:1px solid #e2e8f0;border-radius:12px"></textarea></label>
        <br>
        <button type="submit" class="btn primary" data-i18n="contact.send">Enviar</button>
      </form>
    </section>
  </main>

  <footer>
    <div class="wrap" style="display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap">
      <div>© <span id="year"></span> JE SUIS TRADUTORA. <span data-i18n="footer.rights">Todos os direitos reservados.</span></div>
      <div class="muted">PT • EN • FR • ES</div>
    </div>
  </footer>

  <a class="btn whatsapp" href="https://wa.me/5571999061164" target="_blank" rel="noopener">WhatsApp</a>

  <script>
    // ano dinâmico
    document.getElementById('year').textContent = new Date().getFullYear();

    // Traduções (i18n) — conteúdo chave em quatro idiomas
    const t = {
      pt: {
        'nav.services':'Serviços','nav.portfolio':'Portfólio','nav.about':'Sobre','nav.contact':'Contato','nav.cta':'Pedir orçamento',
        'hero.title':'JE SUIS TRADUTORA','hero.tag':'Tradução profissional para quem precisa de precisão e potência poética.','hero.btn1':'Fale com a gente','hero.badge':'Cobrança por projeto',
        'services.title':'Serviços','services.desc':'Soluções sob medida em linguagem, presença e contexto.',
        'services.items.revisao':'Revisão','services.items.revisaoD':'Aprimoramos estilo, gramática e consistência terminológica.',
        'services.items.traducao':'Tradução','services.items.traducaoD':'PT↔EN↔FR↔ES, com precisão e sensibilidade cultural.',
        'services.items.versao':'Versão','services.items.versaoD':'Adaptamos do português para outros idiomas mantendo voz autoral.',
        'services.items.transcricao':'Transcrição','services.items.transcricaoD':'Registro fiel de áudios e vídeos, com tratamento de falas.',
        'services.items.legendagem':'Legendagem','services.items.legendagemD':'Tradução e revisão de legendas com timing e normas.',
        'services.items.simultanea':'Tradução simultânea','services.items.simultaneaD':'Interpretação em tempo real para eventos e reuniões.',
        'services.items.consecutiva':'Tradução consecutiva','services.items.consecutivaD':'Interpretação com pausas para ambientes técnicos.',
        'services.items.roteiro':'Criação de roteiro','services.items.roteiroD':'Dramaturgia, audiovisual, publicidade, eventos e mais.',
        'services.pairs':'todas as combinações','services.billing':'Cobrança feita por projeto',
        'portfolio.title':'Principais traduções','portfolio.desc':'Uma amostra de trabalhos em cultura, mercado e tecnologia.',
        'portfolio.google':'Versão pt→en de estudos e pesquisas no Brasil: “Afroempreendedorismo”, “Inteligência Artificial” e “Escassez de profissionais de tecnologia”. (2022)',
        'portfolio.ted':'Revisão de legendas em pt e versão pt→en de palestras sobre sustentabilidade, cultura popular e storytelling. (2021–2022)',
        'portfolio.whatsapp':'Versão pt→en de campanhas de lançamento, planejamento de RP e mídia do WhatsApp Brasil. (2022)',
        'portfolio.tiger':'Versão pt→en de campanhas de lançamento de produtos e eventos. (2022)',
        'portfolio.tvv':'Versão pt→en de materiais de comunicação para parceiros internacionais. (2022)',
        'portfolio.ambev':'Versão pt→en de roteiro da cerimônia de apresentação de novos sócios. (2023)',
        'portfolio.hai':'Transcrição e legendagem pt→en do documentário de Antônio Galvão. (2025)',
        'portfolio.boia':'Transcrição e legendagem pt→en do longa de Luiz e Ricardo Pretti. (2025)',
        'portfolio.pax':'Transcrição e legendagem pt→en do documentário dirigido por Nino Franco. (2023)',
        'portfolio.ana':'Versão pt→en da dramaturgia de Mônica Santana. (2023)',
        'portfolio.porto':'Transcrição e legendagem pt→en + pt→es, doc. dirigido por Bernard Attal. (2022)',
        'portfolio.farraial':'Transcrição para a agência InHaus. (2022)',
        'portfolio.catadoras':'Versão pt→en da obra documental. (2021)',
        'about.title':'Sobre a agência','about.text':'A agência nasce do desejo de propor outro espectro na atividade de tradução. Superar limitações técnicas e abandonar a cultura solitária e mecânica. Passear por distintas expressões artísticas além da literatura e observar as alterações linguísticas quase como uma renovação celular vibrando em corpo vivo. Desconstruir gramáticas obsoletas e dar um zoom nas variações regionais, temporais e políticas. Quem está por trás da agência tem histórias fundidas com teatro, escrita, educação e produção cultural e até aqui, traduzimos informações com potencial de alteração da realidade rumo à expansão futurista.',
        'process.1t':'Briefing vivo','process.1d':'Objetivo, público e referências culturais.',
        'process.2t':'Execução especializada','process.2d':'Profissional alinhado ao tema e glossários.',
        'process.3t':'Revisão dupla','process.3d':'Controle de qualidade e padronização.',
        'process.4t':'Entrega & pós','process.4d':'Ajustes finos e suporte após envio.',
        'bio.text':'Rebeca é atriz, tradutora, cronista e roteirista. Lançou “Cotidiano arde e o resto é silêncio” pela editora Urutau e encontra-se em fase de montagem do monólogo autoral “Sugar Baby do Brasil”, com o apoio do IBT e da Funarte. Estreou em 2024 no audiovisual no longa “Vila Buarque” (título em definição) de Luiz e Ricardo Pretti e no curta “Como vivem os mortos” da produtora É Nós na Fita. Traduziu a dramaturgia “Ana e Tadeu” de Mônica Santana e o longa “Porto de Origem” de Bernard Attal. Nos palcos desde 2003, atuou em mais de 20 espetáculos.',
        'cta.title':'Pronto(a) para o próximo projeto?','cta.desc':'Envie arquivo, prazo e objetivo. Retornamos com o orçamento.','cta.btn':'Solicitar orçamento',
        'contact.title':'Contato','contact.desc':'Atendimento seg–sex, 9h–18h (BRT).','contact.billing':'Cobrança feita por projeto.','contact.send':'Enviar',
        'footer.rights':'Todos os direitos reservados.'
      },
      en: {
        'nav.services':'Services','nav.portfolio':'Work','nav.about':'About','nav.contact':'Contact','nav.cta':'Request a quote',
        'hero.title':'JE SUIS TRADUTORA','hero.tag':'Professional translation with precision and poetic power.','hero.btn1':'Talk to us','hero.badge':'Project-based pricing',
        'services.title':'Services','services.desc':'Tailored language, presence and context solutions.',
        'services.items.revisao':'Editing & Proofreading','services.items.revisaoD':'Style, grammar and terminology consistency.',
        'services.items.traducao':'Translation','services.items.traducaoD':'PT↔EN↔FR↔ES, with cultural sensitivity.',
        'services.items.versao':'Version (PT→other)','services.items.versaoD':'From Portuguese into other languages, preserving voice.',
        'services.items.transcricao':'Transcription','services.items.transcricaoD':'Accurate transcripts for audio and video.',
        'services.items.legendagem':'Subtitling','services.items.legendagemD':'Translation and QC of subtitles (timing & standards).',
        'services.items.simultanea':'Simultaneous interpreting','services.items.simultaneaD':'Real-time for events and meetings.',
        'services.items.consecutiva':'Consecutive interpreting','services.items.consecutivaD':'With pauses for technical settings.',
        'services.items.roteiro':'Scriptwriting','services.items.roteiroD':'Stage, audiovisual, advertising, events and more.',
        'services.pairs':'all language pairs','services.billing':'Project-based pricing',
        'portfolio.title':'Selected work','portfolio.desc':'A sample across culture, markets and tech.',
        'portfolio.google':'PT→EN versions of studies in Brazil: “Afro-entrepreneurship”, “Artificial Intelligence” and “Tech talent shortage”. (2022)',
        'portfolio.ted':'Subtitle review in PT and PT→EN for talks on sustainability, popular culture and storytelling. (2021–2022)',
        'portfolio.whatsapp':'PT→EN for launch campaigns, PR and media planning for WhatsApp Brazil. (2022)',
        'portfolio.tiger':'PT→EN for product launch campaigns and events. (2022)',
        'portfolio.tvv':'PT→EN for communication materials for international partners. (2022)',
        'portfolio.ambev':'PT→EN of the ceremony script introducing new partners. (2023)',
        'portfolio.hai':'Transcription and subtitling PT→EN of Antônio Galvão’s documentary. (2025)',
        'portfolio.boia':'Transcription and subtitling PT→EN of the feature by Luiz & Ricardo Pretti. (2025)',
        'portfolio.pax':'Transcription and subtitling PT→EN of the documentary directed by Nino Franco. (2023)',
        'portfolio.ana':'PT→EN of Mônica Santana’s play. (2023)',
        'portfolio.porto':'Transcription and subtitling PT→EN + PT→ES of Bernard Attal’s documentary. (2022)',
        'portfolio.farraial':'Transcription for InHaus agency. (2022)',
        'portfolio.catadoras':'PT→EN of the documentary work. (2021)',
        'about.title':'About the agency','about.text':'The agency was born from a desire to open a new spectrum in translation practice: to transcend technical limits and leave behind a solitary, mechanical culture. We move through artistic expressions beyond literature and observe linguistic change as a living body’s renewal. We deconstruct obsolete grammars and zoom into regional, temporal and political variations. Our background blends theatre, writing, education and cultural production, translating information with the power to shift reality toward a futuristic expansion.',
        'process.1t':'Live briefing','process.1d':'Purpose, audience and cultural references.',
        'process.2t':'Specialised execution','process.2d':'Professional aligned with the topic and glossaries.',
        'process.3t':'Dual review','process.3d':'Quality control and standardisation.',
        'process.4t':'Delivery & aftercare','process.4d':'Fine tuning and support after delivery.',
        'bio.text':'Rebeca is an actress, translator, columnist and screenwriter. She published “Cotidiano arde e o resto é silêncio” (Urutau) and is staging her solo “Sugar Baby do Brasil” with support from IBT and Funarte. In 2024 she debuted on screen in the feature “Vila Buarque” (working title) by Luiz & Ricardo Pretti and in the short “Como vivem os mortos” (É Nós na Fita). She translated the play “Ana e Tadeu” by Mônica Santana and the documentary feature “Porto de Origem” by Bernard Attal. On stage since 2003, she has performed in over 20 productions.',
        'cta.title':'Ready for the next project?','cta.desc':'Send file, deadline and context. We will quote back.','cta.btn':'Request a quote',
        'contact.title':'Contact','contact.desc':'Mon–Fri, 9am–6pm (BRT).','contact.billing':'Project-based pricing.','contact.send':'Send',
        'footer.rights':'All rights reserved.'
      },
      fr: {
        'nav.services':'Services','nav.portfolio':'Références','nav.about':'À propos','nav.contact':'Contact','nav.cta':'Demander un devis',
        'hero.title':'JE SUIS TRADUTORA','hero.tag':'Traduction professionnelle alliant précision et puissance poétique.','hero.btn1':'Parlez-nous','hero.badge':'Tarification par projet',
        'services.title':'Services','services.desc':'Solutions sur mesure en langue, présence et contexte.',
        'services.items.revisao':'Révision','services.items.revisaoD':'Style, grammaire et cohérence terminologique.',
        'services.items.traducao':'Traduction','services.items.traducaoD':'PT↔EN↔FR↔ES avec sensibilité culturelle.',
        'services.items.versao':'Version (PT→autres)','services.items.versaoD':'Du portugais vers d’autres langues en préservant la voix.',
        'services.items.transcricao':'Transcription','services.items.transcricaoD':'Transcriptions précises audio et vidéo.',
        'services.items.legendagem':'Sous-titrage','services.items.legendagemD':'Traduction et QC des sous-titres (timing et normes).',
        'services.items.simultanea':'Interprétation simultanée','services.items.simultaneaD':'En temps réel pour événements et réunions.',
        'services.items.consecutiva':'Interprétation consécutive','services.items.consecutivaD':'Avec pauses pour contextes techniques.',
        'services.items.roteiro':'Écriture de scénarios','services.items.roteiroD':'Dramaturgie, audiovisuel, publicité, événements, etc.',
        'services.pairs':'toutes les combinaisons','services.billing':'Tarification par projet',
        'portfolio.title':'Références principales','portfolio.desc':'Un échantillon dans la culture, le marché et la tech.',
        'portfolio.google':'Versions PT→EN d’études au Brésil : « Afro-entrepreneuriat », « Intelligence artificielle » et « Pénurie de talents tech ». (2022)',
        'portfolio.ted':'Révision de sous-titres en PT et PT→EN pour des conférences sur la durabilité, la culture populaire et le storytelling. (2021–2022)',
        'portfolio.whatsapp':'PT→EN pour campagnes de lancement, RP et médias de WhatsApp Brésil. (2022)',
        'portfolio.tiger':'PT→EN pour campagnes de lancement et événements. (2022)',
        'portfolio.tvv':'PT→EN pour supports de communication à destination de partenaires internationaux. (2022)',
        'portfolio.ambev':'PT→EN du script de cérémonie présentant de nouveaux associés. (2023)',
        'portfolio.hai':'Transcription et sous-titrage PT→EN du documentaire d’Antônio Galvão. (2025)',
        'portfolio.boia':'Transcription et sous-titrage PT→EN du long métrage de Luiz & Ricardo Pretti. (2025)',
        'portfolio.pax':'Transcription et sous-titrage PT→EN du documentaire de Nino Franco. (2023)',
        'portfolio.ana':'PT→EN de la pièce de Mônica Santana. (2023)',
        'portfolio.porto':'Transcription et sous-titrage PT→EN + PT→ES du documentaire de Bernard Attal. (2022)',
        'portfolio.farraial':'Transcription pour l’agence InHaus. (2022)',
        'portfolio.catadoras':'PT→EN de l’œuvre documentaire. (2021)',
        'about.title':'À propos de l’agence','about.text':'L’agence naît du désir d’ouvrir un autre spectre de la traduction : dépasser les limites techniques et quitter une culture solitaire et mécanique. Nous circulons entre diverses expressions artistiques au-delà de la littérature et observons le changement linguistique comme une régénération d’un corps vivant. Nous déconstruisons des grammaires obsolètes et faisons le zoom sur les variations régionales, temporelles et politiques. Nos parcours mêlent théâtre, écriture, éducation et production culturelle ; nous traduisons des informations susceptibles de transformer la réalité vers une expansion futuriste.',
        'process.1t':'Brief vivant','process.1d':'Objectif, public et références culturelles.',
        'process.2t':'Exécution spécialisée','process.2d':'Professionnel aligné au sujet et glossaires.',
        'process.3t':'Double révision','process.3d':'Contrôle qualité et standardisation.',
        'process.4t':'Livraison & suivi','process.4d':'Ajustements fins et support après livraison.',
        'bio.text':'Rebeca est actrice, traductrice, chroniqueuse et scénariste. Elle a publié « Cotidiano arde e o resto é silêncio » (Urutau) et monte son solo « Sugar Baby do Brasil », avec le soutien de l’IBT et de la Funarte. En 2024, elle débute à l’écran dans le long métrage « Vila Buarque » (titre provisoire) de Luiz & Ricardo Pretti et dans le court « Como vivem os mortos ». Elle a traduit la pièce « Ana e Tadeu » (Mônica Santana) et le documentaire « Porto de Origem » (Bernard Attal). Sur scène depuis 2003, elle a joué dans plus de 20 spectacles.',
        'cta.title':'Prêt·e pour le prochain projet ?','cta.desc':'Envoyez fichier, délai et objectif. Nous revenons avec un devis.','cta.btn':'Demander un devis',
        'contact.title':'Contact','contact.desc':'Lun–Ven, 9h–18h (BRT).','contact.billing':'Tarification par projet.','contact.send':'Envoyer',
        'footer.rights':'Tous droits réservés.'
      },
      es: {
        'nav.services':'Servicios','nav.portfolio':'Portafolio','nav.about':'Sobre','nav.contact':'Contacto','nav.cta':'Pedir presupuesto',
        'hero.title':'JE SUIS TRADUTORA','hero.tag':'Traducción profesional con precisión y potencia poética.','hero.btn1':'Hable con nosotros','hero.badge':'Cobro por proyecto',
        'services.title':'Servicios','services.desc':'Soluciones a medida en lengua, presencia y contexto.',
        'services.items.revisao':'Revisión','services.items.revisaoD':'Estilo, gramática y consistencia terminológica.',
        'services.items.traducao':'Traducción','services.items.traducaoD':'PT↔EN↔FR↔ES con sensibilidad cultural.',
        'services.items.versao':'Versión (PT→otros)','services.items.versaoD':'Del portugués a otros idiomas manteniendo la voz.',
        'services.items.transcricao':'Transcripción','services.items.transcricaoD':'Registros fieles de audio y video.',
        'services.items.legendagem':'Subtitulación','services.items.legendagemD':'Traducción y control de calidad de subtítulos.',
        'services.items.simultanea':'Interpretación simultánea','services.items.simultaneaD':'En tiempo real para eventos y reuniones.',
        'services.items.consecutiva':'Interpretación consecutiva','services.items.consecutivaD':'Con pausas para entornos técnicos.',
        'services.items.roteiro':'Creación de guion','services.items.roteiroD':'Dramaturgia, audiovisual, publicidad, eventos y más.',
        'services.pairs':'todas las combinaciones','services.billing':'Cobro por proyecto',
        'portfolio.title':'Trabajos destacados','portfolio.desc':'Una muestra en cultura, mercado y tecnología.',
        'portfolio.google':'Versión PT→EN de estudios en Brasil: “Afroemprendimiento”, “Inteligencia Artificial” y “Escasez de talento tech”. (2022)',
        'portfolio.ted':'Revisión de subtítulos en PT y PT→EN de charlas sobre sostenibilidad, cultura popular y storytelling. (2021–2022)',
        'portfolio.whatsapp':'PT→EN para campañas de lanzamiento, RP y planificación de medios de WhatsApp Brasil. (2022)',
        'portfolio.tiger':'PT→EN para campañas de lanzamiento y eventos. (2022)',
        'portfolio.tvv':'PT→EN para materiales de comunicación a socios internacionales. (2022)',
        'portfolio.ambev':'PT→EN del guion de ceremonia presentando nuevos socios. (2023)',
        'portfolio.hai':'Transcripción y subtitulación PT→EN del documental de Antônio Galvão. (2025)',
        'portfolio.boia':'Transcripción y subtitulación PT→EN del largometraje de Luiz y Ricardo Pretti. (2025)',
        'portfolio.pax':'Transcripción y subtitulación PT→EN del documental dirigido por Nino Franco. (2023)',
        'portfolio.ana':'PT→EN de la dramaturgia de Mônica Santana. (2023)',
        'portfolio.porto':'Transcripción y subtitulación PT→EN + PT→ES del documental de Bernard Attal. (2022)',
        'portfolio.farraial':'Transcripción para la agencia InHaus. (2022)',
        'portfolio.catadoras':'PT→EN de la obra documental. (2021)',
        'about.title':'Sobre la agencia','about.text':'La agencia nace del deseo de proponer otro espectro en la traducción: superar limitaciones técnicas y abandonar una cultura solitaria y mecánica. Paseamos por expresiones artísticas más allá de la literatura y observamos los cambios lingüísticos como la renovación de un cuerpo vivo. Deconstruimos gramáticas obsoletas y hacemos zoom en variaciones regionales, temporales y políticas. Detrás de la agencia hay trayectorias en teatro, escritura, educación y producción cultural; traducimos información con potencial de alterar la realidad hacia una expansión futurista.',
        'process.1t':'Briefing vivo','process.1d':'Objetivo, público y referencias culturales.',
        'process.2t':'Ejecución especializada','process.2d':'Profesional alineado al tema y glosarios.',
        'process.3t':'Doble revisión','process.3d':'Control de calidad y estandarización.',
        'process.4t':'Entrega y posventa','process.4d':'Ajustes finos y soporte posterior.',
        'bio.text':'Rebeca es actriz, traductora, columnista y guionista. Publicó “Cotidiano arde e o resto é silêncio” (Urutau) y está montando el unipersonal “Sugar Baby do Brasil”, con apoyo del IBT y Funarte. En 2024 debutó en cine en el largometraje “Vila Buarque” (título en definición) de Luiz y Ricardo Pretti y en el corto “Como vivem os mortos”. Tradujo la obra “Ana e Tadeu” de Mônica Santana y el documental “Porto de Origem” de Bernard Attal. En escena desde 2003, actuó en más de 20 espectáculos.',
        'cta.title':'¿Lista/o para el próximo proyecto?','cta.desc':'Envíe archivo, plazo y objetivo. Volvemos con presupuesto.','cta.btn':'Pedir presupuesto',
        'contact.title':'Contacto','contact.desc':'Lun–Vie, 9h–18h (BRT).','contact.billing':'Cobro por proyecto.','contact.send':'Enviar',
        'footer.rights':'Todos los derechos reservados.'
      }
    };

    const el = document.querySelectorAll('[data-i18n]');
    const select = document.getElementById('lang');
    function apply(lang){
      el.forEach(node=>{ const k=node.getAttribute('data-i18n'); if(t[lang]&&t[lang][k]) node.textContent=t[lang][k]; });
      document.documentElement.lang = lang;
    }
    select.addEventListener('change', e=>apply(e.target.value));
    // inicia PT
    apply('pt');
  </script>
</body>
</html>
