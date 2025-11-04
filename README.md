# MikaWeb
site mikaweb
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MikaWeb</title>
  <meta name="description" content="MikaWeb — Site personnel moderne et élégant">

  <style>
    :root {
      --fond: #050505;
      --carte: #121212;
      --accent: #9b1cff;
      --rouge: #d00000;
      --violet: #6a00ff;
      --texte: #e0e0e0;
      --muted: #a0a0a0;
      --verre: rgba(255,255,255,0.05);
    }

    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: var(--fond);
      color: var(--texte);
      line-height: 1.5;
    }

    .conteneur { max-width: 1100px; margin: 0 auto; padding: 24px; }
    header { display: flex; align-items: center; justify-content: space-between; padding: 12px 0; }
    .marque { display: flex; align-items: center; gap: 12px; }
    .logo {
      width: 80px;
      height: 80px;
      border-radius: 20px;
      background: linear-gradient(135deg, var(--rouge), var(--violet));
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 36px;
      font-weight: 700;
      color: #fff;
      box-shadow: 0 0 25px rgba(107,0,255,0.5);
    }

    nav ul { display: flex; gap: 18px; list-style: none; padding: 0; margin: 0; }
    nav a { color: var(--muted); text-decoration: none; transition: color .2s; }
    nav a:hover { color: var(--accent); }
    .cta { background: var(--accent); color: #000; padding: 10px 14px; border-radius: 10px; font-weight: 600; text-decoration: none; }

    .hero {
      text-align: center;
      padding: 80px 20px;
      background: #1a1a1a;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(0,0,0,0.7);
    }

    .hero h1 {
      font-size: 52px;
      margin: 20px 0;
      background: linear-gradient(90deg, var(--rouge), var(--violet));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      font-weight: 800;
      text-shadow: 0 0 25px rgba(155,28,255,0.3);
    }

    .hero p { color: #ddd; font-size: 18px; max-width: 600px; margin: 0 auto; }
    .citation { margin-top: 20px; font-style: italic; font-size: 20px; color: #fff; }

    .shadow-image { margin-top: 20px; width: 60%; border-radius: 12px; box-shadow: 0 0 30px rgba(107,0,255,0.5); }

    .grille { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin: 50px 0; }
    .carte { background: var(--carte); padding: 20px; border-radius: 12px; box-shadow: 0 4px 16px rgba(0,0,0,0.5); }
    .carte h3 { margin: 0 0 8px; }
    .muted { color: var(--muted); }
    #a-propos img { width: 100%; border-radius: 12px; margin-bottom: 12px; }

    form input, form textarea {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid rgba(255,255,255,0.04);
      background: var(--verre);
      color: inherit;
    }

    form button {
      margin-top: 8px;
      padding: 10px 14px;
      border-radius: 8px;
      border: 0;
      background: var(--accent);
      color: #000;
      cursor: pointer;
      font-weight: 600;
    }

    footer {
      border-top: 1px solid rgba(255,255,255,0.1);
      padding: 18px 0;
      margin-top: 36px;
      text-align: center;
      color: var(--muted);
    }
  </style>
</head>

<body>
  <div class="conteneur">
    <header>
      <div class="marque">
        <div class="logo">Mk</div>
        <div>
          <div style="font-weight:700;font-size:22px">MikaWeb</div>
          <div class="muted">Création & inspiration numérique</div>
        </div>
      </div>
      <nav>
        <ul>
          <li><a href="#accueil">Accueil</a></li>
          <li><a href="#fonctionnalites">Fonctionnalités</a></li>
          <li><a href="#a-propos">À propos</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <a class="cta" href="#contact">Me contacter</a>
    </header>

    <section id="accueil" class="hero">
      <div class="logo" style="margin:0 auto; width:120px; height:120px; font-size:60px;">Mk</div>
      <h1>Bienvenue sur MikaWeb</h1>
      <p>Un site personnel moderne avec un style sombre, inspiré de l’univers de The Eminence in Shadow.</p>
      <div class="citation">Nous sommes un empire uni pour la victoire — <strong>“One for all”</strong> — solitaire mais toujours uni.</div>
      <!-- Images de The Eminence in Shadow -->
      <img class="shadow-image" src="https://practicaltyping.com/wp-content/uploads/2024/01/cidkagenou.png" alt="Shadow - The Eminence in Shadow" />
      <img class="shadow-image" src="https://shadow-garden.jp/assets/img/common/visual2.jpg" alt="Shadow - The Eminence in Shadow" />
    </section>

    <section id="fonctionnalites">
      <h2>Fonctionnalités</h2>
      <div class="grille">
        <div class="carte"><h3>Design sombre</h3><p class="muted">Une interface élégante, agréable pour les yeux.</p></div>
        <div class="carte"><h3>Adaptatif</h3><p class="muted">Le site s’adapte à tous les écrans : mobile, tablette, ordinateur.</p></div>
        <div class="carte"><h3>Personnalisable</h3><p class="muted">Change les couleurs, les images et les textes selon tes goûts.</p></div>
      </div>
    </section>

    <section id="a-propos">
      <h2>À propos</h2>
      <div class="carte">
        <img src="https://practicaltyping.com/wp-content/uploads/2024/01/cidkagenou.png" alt="Shadow - The Eminence in Shadow" />
        <p class="muted">MikaWeb est un projet personnel pour expérimenter le développement web, le design et la création de contenus. J’aime apprendre, créer et partager mes découvertes avec le monde.</p>
      </div>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <div class="grille">
        <div class="carte">
          <form onsubmit="envoyerMessage(event)">
            <label>Nom</label>
            <input required placeholder="Ex: Mika" />
            <label>Email</label>
            <input type="email" required placeholder="vous@example.com" />
            <label>Message</label>
            <textarea rows="5" placeholder="Votre message..."></textarea>
            <button type="submit">Envoyer</button>
          </form>
        </div>
        <div class="carte">
          <h3>Mes réseaux</h3>
          <p class="muted">Tu peux me retrouver sur : <br> 💼 LinkedIn — 📸 Instagram — 🐦 Twitter</p>
        </div>
      </div>
    </section>

    <footer>
      © <span id="annee"></span> MikaWeb — Créé avec ❤️ et passion.
    </footer>
  </div>

  <script>
    document.getElementById('annee').textContent = new Date().getFullYear();

    function envoyerMessage(e){
      e.preventDefault();
      alert('Merci pour