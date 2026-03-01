# paul.net
Mon portfolio personnel
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Paul Christi Ngandziami Mbissi - Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #0f172a, #1e293b);
    color: white;
    scroll-behavior: smooth;
}

/* NAVBAR */

nav {
    position: fixed;
    width: 100%;
    background: rgba(0,0,0,0.7);
    backdrop-filter: blur(10px);
    padding: 15px 0;
    text-align: center;
    z-index: 1000;
}

nav a {
    color: white;
    margin: 0 20px;
    text-decoration: none;
    font-weight: 500;
    transition: 0.3s;
}

nav a:hover {
    color: #38bdf8;
}

/* HEADER */

header {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    animation: fadeIn 2s ease;
}

header h1 {
    font-size: 45px;
}

header p {
    margin-top: 15px;
    font-size: 20px;
    color: #38bdf8;
}

/* SECTIONS */

section {
    padding: 100px 20px;
    max-width: 1000px;
    margin: auto;
}

h2 {
    margin-bottom: 20px;
    color: #38bdf8;
    font-size: 28px;
}

.card {
    background: rgba(255,255,255,0.05);
    padding: 30px;
    border-radius: 15px;
    backdrop-filter: blur(15px);
    margin-top: 20px;
    transition: transform 0.4s ease, box-shadow 0.4s ease;
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 0 25px rgba(56,189,248,0.4);
}

ul {
    line-height: 1.8;
}

/* BUTTON */

.btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    border-radius: 25px;
    background: #38bdf8;
    color: #0f172a;
    font-weight: 600;
    text-decoration: none;
    transition: 0.3s;
}

.btn:hover {
    background: white;
}

/* FOOTER */

footer {
    text-align: center;
    padding: 30px;
    background: #020617;
}

/* ANIMATION */

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
}

/* SCROLL ANIMATION */

.hidden {
    opacity: 0;
    transform: translateY(40px);
    transition: all 1s;
}

.show {
    opacity: 1;
    transform: translateY(0);
}

</style>
</head>

<body>

<nav>
<a href="#about">À propos</a>
<a href="#skills">Compétences</a>
<a href="#projects">Projets</a>
<a href="#docs">Documentation</a>
<a href="#contact">Contact</a>
</nav>

<header>
<h1>Paul Christi Ngandziami Mbissi</h1>
<p>BTS SIO - Option SISR</p>
</header>

<section id="about" class="hidden">
<h2>À propos de moi</h2>
<div class="card">
Je suis étudiant en BTS SIO option SISR, passionné par les systèmes, les réseaux et la sécurité informatique.
Je développe mes compétences à travers des projets concrets en environnement virtualisé et infrastructure réseau.
</div>
</section>

<section id="skills" class="hidden">
<h2>Compétences techniques</h2>
<div class="card">
<ul>
<li>Administration Windows Server</li>
<li>Configuration DNS & DHCP</li>
<li>Active Directory (utilisateurs, groupes, GPO)</li>
<li>Installation et configuration pfSense</li>
<li>Déploiement GLPI</li>
<li>Virtualisation VMware</li>
<li>Topologies réseau (Packet Tracer)</li>
<li>Tests et diagnostic de connectivité</li>
</ul>
</div>
</section>

<section id="projects" class="hidden">
<h2>Projet réalisé</h2>
<div class="card">
<h3>Infrastructure réseau virtualisée</h3>
<ul>
<li>Installation Windows Server sur VMware</li>
<li>Configuration DNS & DHCP</li>
<li>Mise en place Active Directory</li>
<li>Installation et configuration pfSense</li>
<li>Déploiement GLPI</li>
<li>Topologie : 2 PC + Switch</li>
<li>Tests de connectivité et validation réseau</li>
</ul>
</div>
</section>

<section id="docs" class="hidden">
<h2>Documentation</h2>
<div class="card">
<a class="btn" href="cv.pdf" target="_blank">Télécharger CV</a><br>
<a class="btn" href="tableau_synthese.pdf" target="_blank">Tableau de synthèse</a><br>
<a class="btn" href="documentation_projet.pdf" target="_blank">Documentation projet</a>
</div>
</section>

<section id="contact" class="hidden">
<h2>Contact</h2>
<div class="card">
<p>Email : <a href="mailto:christipaul14@gmail.com" style="color:#38bdf8;">christipaul14@gmail.com</a></p>
<p>Téléphone : <a href="tel:+33745611694" style="color:#38bdf8;">+33 7 45 61 16 94</a></p>
</div>
</section>

<footer>
© 2026 - Paul Christi Ngandziami Mbissi
</footer>

<script>
const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if(entry.isIntersecting){
            entry.target.classList.add("show");
        }
    });
});

document.querySelectorAll('.hidden').forEach(el => observer.observe(el));
</script>

</body>
</html>
