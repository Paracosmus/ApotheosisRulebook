---
label: Home
layout: page
---

<style>
    /* ANIMAÇÕES */
    @keyframes pulse-glow {
        0% { box-shadow: 0 0 0 0 rgba(103, 58, 183, 0.4); }
        70% { box-shadow: 0 0 0 15px rgba(103, 58, 183, 0); }
        100% { box-shadow: 0 0 0 0 rgba(103, 58, 183, 0); }
    }

    img {
        border: 3px solid rgba(0, 28, 112, 0.2);
    }

    /* HERO SECTION */
    .hero-section {
        text-align: center;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
        margin: 1rem 0;
        padding: 2rem 1rem;
        background: radial-gradient(ellipse at top, rgba(15, 9, 26, 0.15), transparent 70%);
        border-radius: 20px;
    }
    .hero-title {
        font-size: 2.5em;
        font-weight: 900;
        background: linear-gradient(45deg, #000000, #2196F3);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        display: block;
        padding-bottom: 0px;
        margin-bottom: 1rem;
        line-height: 1.2;
        text-align: center !important;
        width: 100%;
        text-shadow: 0 4px 20px rgba(103, 58, 183, 0.2);
        letter-spacing: 1px;
    }
    .hero-subtitle {
        font-size: 1.5rem;
        color: #888;
        font-weight: 300;
        margin-bottom: 1rem;
    }
    .author-badge {
        display: inline-block;
        padding: 5px 15px;
        background: rgba(33, 150, 243, 0.1);
        color: #2196F3;
        border-radius: 20px;
        font-weight: 600;
        font-size: 0.9rem;
        margin-bottom: 1rem;
        border: 1px solid rgba(33, 150, 243, 0.3);
        box-shadow: 0 4px 10px rgba(33, 150, 243, 0.1);
        transition: all 0.3s ease;
    }
    .author-badge:hover {
        background: rgba(33, 150, 243, 0.2);
        transform: translateY(-2px);
        box-shadow: 0 6px 15px rgba(33, 150, 243, 0.2);
    }
    .intro-text {
        font-size: 1.15rem;
        line-height: 1.6;
        text-align: center;
        max-width: 750px;
        margin: 0 auto 3rem auto;
        color: var(--color-text-secondary, #888);
    }

    /* GRID DE PILARES */
    .pillars-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1.5rem;
        margin: 2rem 0;
    }
    @media (max-width: 768px) {
        .pillars-grid {
            grid-template-columns: 1fr;
        }
    }
    .pillar-card {
        background: linear-gradient(145deg, rgba(128, 128, 128, 0.05) 0%, rgba(128, 128, 128, 0.01) 100%);
        border: 2px solid rgba(255, 255, 255, 0.75);
        border-radius: 16px;
        padding: 2rem 1.5rem;
        text-align: center;
        transition: all 0.3s ease;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
        backdrop-filter: blur(10px);
    }
    .pillar-card:hover {
        transform: translateY(-8px);
        border-color: #7790f6;
        box-shadow: 0 15px 35px rgba(103, 58, 183, 0.15);
        background: linear-gradient(145deg, rgba(103, 58, 183, 0.05) 0%, rgba(33, 150, 243, 0.05) 100%);
    }
    .pillar-icon {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        width: 70px;
        height: 70px;
        font-size: 2.5rem;
        margin-bottom: 1.5rem;
        background: linear-gradient(135deg, rgba(103, 58, 183, 0.1), rgba(33, 150, 243, 0.1));
        border-radius: 50%;
        box-shadow: inset 0 0 20px rgba(255, 255, 255, 0.02), 0 8px 16px rgba(0, 0, 0, 0.05);
        transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }
    .pillar-card:hover .pillar-icon {
        transform: scale(1.15) rotate(5deg);
    }
    .pillar-svg {
        width: 36px;
        height: 36px;
        stroke: url(#icon-gradient);
        stroke-width: 1.5;
        fill: none;
        transition: all 0.3s ease;
    }
    .pillar-card:hover .pillar-svg {
        stroke-width: 2;
        filter: drop-shadow(0px 0px 6px rgba(103, 58, 183, 0.4));
    }
    .pillar-title {
        font-size: 1.25rem;
        font-weight: bold;
        margin-bottom: 1rem;
    }
    .pillar-desc {
        font-size: 0.95rem;
        opacity: 0.8;
        line-height: 1.5;
    }

    /* CALL TO ACTION */
    .cta-container {
        text-align: center;
        margin-top: 8rem;
        padding: 0rem 1.5rem;
        background: linear-gradient(135deg, rgba(221, 226, 255, 0.08), rgba(163, 211, 251, 0.08));
        border-radius: 24px;
        border: 1px solid rgba(32, 32, 123, 0.2);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.05);
        position: relative;
        overflow: hidden;
    }
    .cta-title {
        font-size: 2rem;
        font-weight: 800;
        margin-bottom: 1rem;
        background: linear-gradient(to right, #673AB7, #2196F3);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }
</style>

![](static/img/banner.jpg){.rounded-lg}

<div class="hero-section">
    <div class="hero-title" role="heading" aria-level="1">APOTHEOSIS CARD GAME</div>
    <div class="author-badge">Criado por Bruno Caxito</div>
</div>

<div class="intro-text">
    <p><b>APOTHEOSIS CARD GAME</b> é um jogo de cartas modular que combina elementos de <i>role-playing game</i> (RPG), construção de baralho e batalha em um tabuleiro quadriculado, ambientado em um universo próprio com história e narrativa únicas.</p>
    <p>Jogadores coletam cartas para compor seu personagem, que pode enfrentar desafios propostos por uma campanha narrativa ou batalhar contra os personagens de outros jogadores pela vitória.</p>
</div>

---

<h2 style="text-align: center; margin-top: 3rem; margin-bottom: 1rem;">Arquitetura do Sistema</h2>

<svg style="width:0; height:0; position:absolute;" aria-hidden="true">
    <defs>
        <linearGradient id="icon-gradient" x1="0%" y1="0%" x2="100%" y2="100%">
            <stop offset="0%" stop-color="#673AB7" />
            <stop offset="100%" stop-color="#2196F3" />
        </linearGradient>
    </defs>
</svg>

<div class="pillars-grid">
    <div class="pillar-card">
        <div class="pillar-icon">
            <svg class="pillar-svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round">
                <rect x="3" y="7" width="13" height="14" rx="2" ry="2"></rect>
                <path d="M8 3h11a2 2 0 0 1 2 2v11"></path>
            </svg>
        </div>
        <div class="pillar-title">Cartas e Baralhos</div>
        <div class="pillar-desc">O núcleo do jogo. Representam habilidades, itens, magias e eventos. Combine recursos e crie sinergias perfeitas para superar seus limites.</div>
    </div>
    <div class="pillar-card">
        <div class="pillar-icon">
            <svg class="pillar-svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round">
                <path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path>
                <circle cx="12" cy="7" r="4"></circle>
            </svg>
        </div>
        <div class="pillar-title">Heróis e Personagens</div>
        <div class="pillar-desc">Você não é apenas um jogador, é um Herói. Evolua cartas de Classe, Casa e Ente para moldar um personagem com habilidades e atributos únicos.</div>
    </div>
    <div class="pillar-card">
        <div class="pillar-icon">
            <svg class="pillar-svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round">
                <rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect>
                <path d="M3 9h18M3 15h18M9 3v18M15 3v18"></path>
            </svg>
        </div>
        <div class="pillar-title">Tabuleiro e Batalhas</div>
        <div class="pillar-desc">A ação acontece em um espaço quadriculado. O posicionamento, o controle de área e o alcance são tão vitais quanto as cartas que você escolhe jogar.</div>
    </div>
    <div class="pillar-card">
        <div class="pillar-icon">
            <svg class="pillar-svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round">
                <path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"></path>
                <path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"></path>
            </svg>
        </div>
        <div class="pillar-title">Narrativa e Testes</div>
        <div class="pillar-desc">Mergulhe em um mundo rico. Cumpra objetivos cooperativos contra ameaças em campanhas ou enfrente seus rivais nos competitivos modos de Arena.</div>
    </div>
</div>

<div class="cta-container">

[!ref Getting Started](/getting-started.md)

</div>
