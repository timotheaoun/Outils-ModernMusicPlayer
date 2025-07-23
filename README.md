<!DOCTYPE html>

<html lang="fr">

<head>

<meta charset="UTF-8" />

<meta name="viewport" content="width=device-width, initial-scale=1" />

<title>À propos - Notre service</title>



<style>

  /* Reset CSS minimal */

  *, *::before, *::after {

    box-sizing: border-box;

  }



  body {

    margin: 0;

    background: #121212;

    color: #eee;

    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

    line-height: 1.6;

    -webkit-font-smoothing: antialiased;

    -moz-osx-font-smoothing: grayscale;

    min-height: 100vh;

    display: flex;

    flex-direction: column;

  }



  header {

    background: linear-gradient(90deg, #0f2027, #203a43, #2c5364);

    padding: 2rem 1.5rem;

    text-align: center;

    box-shadow: 0 4px 15px rgba(0,0,0,0.6);

  }

  header h1 {

    font-weight: 900;

    font-size: 2.8rem;

    letter-spacing: 0.05em;

    margin: 0;

    color: #fff;

    text-transform: uppercase;

  }

  header p {

    margin-top: 0.5rem;

    font-weight: 500;

    font-size: 1.1rem;

    color: #a3b1c1;

  }



  main {

    max-width: 900px;

    margin: 3rem auto;

    padding: 0 1.5rem 4rem;

  }



  h2 {

    font-size: 2.4rem;

    font-weight: 700;

    margin-bottom: 1rem;

    color: #08fdd8;

    border-left: 5px solid #08fdd8;

    padding-left: 0.8rem;

  }



  p {

    font-size: 1.2rem;

    color: #d0d7de;

    margin-bottom: 1.5rem;

  }



  strong {

    color: #fff;

  }



  ul {

    list-style: inside disc;

    margin-left: 1rem;

    margin-bottom: 1.5rem;

    color: #c7cacc;

  }



  a {

    color: #08fdd8;

    text-decoration: none;

    transition: color 0.3s ease;

  }

  a:hover,

  a:focus {

    color: #5af9e3;

    text-decoration: underline;

    outline: none;

  }



  footer {

    margin-top: auto;

    background: #1e1e1e;

    color: #555;

    text-align: center;

    padding: 1rem 0;

    font-size: 0.9rem;

    user-select: none;

  }



  /* Responsive */

  @media (max-width: 600px) {

    header h1 {

      font-size: 2rem;

    }

    main {

      margin: 2rem 1rem;

      padding-bottom: 3rem;

    }

    h2 {

      font-size: 1.8rem;

    }

    p, ul {

      font-size: 1rem;

    }

  }

</style>

</head>



<body>

<header>

  <h1>À propos de Modern Music Player</h1>

  <p>Un outil en ligne pour apprendre facilement le HTML en injectant du code dans un input, vous pouvez bien entendu l'utiliser comme lecteur de musique...</p>

</header>



<main>

  <section>

    <h2>Ma mission</h2>

    <p>

      Bonjour, je me présente, je suis <strong>Timothé AOUN</strong>. 

	  <br> Je suis passionné par la programmation, les maths et le hacking. Mon objectif est de pouvoir transmettre mon savoir et surtout d'apprendre en vous apprenant, me former en vous formant. C'est pourquoi, sur mon <a href="https://timotheaoun.github.io/">Site wen</a>, vous retrouverez plusieurs projets mathématiques et informatiques qui valent le coup d'oeil.

	  <br><strong>Modern Music Player</strong> est un outil que j'ai initialement conçu à usage personnel, pour écouter de la musique. Remarquant une énorme faille html, j'ai décidé de la concerver et d'en faire un 'bac à sable' en quelque sorte, dans lequel vous pouvez injecter du code.

    </p>

  </section>



  <section>

    <h2>Ce que vous trouverez ici</h2>

    <p>

      Cette page <em>« À propos »</em> a pour but de vous expliquer en détail les subtilités de l'outil:

	  <ul>

      <li><strong>Interface Moderne :</strong> design épuré, thème sombre, simplement pour être agréable</li>

      <li><strong>Performance :</strong> chargement rapide, navigation fluide.</li>

      <li><strong>Apprentissage :</strong> Apprenez à maitriser le html et ses failles à travers un exemple d'outil en ligne très facilement détournable. Je précise que je fais cela dans un but éducatif, l'objectif n'étant pas de vous apprendre le hacking, mais de vous faire cerner son mode de fontionnement afin que vous puissiez mieux vous en protéger</li>

    </ul>

  </section>



<section>

  <h2>Fonctionnement</h2>

  <p>

    Une <strong>faille</strong> en informatique désigne une vulnérabilité ou une faiblesse dans un logiciel ou une application qui peut être exploitée par un attaquant pour causer un comportement non prévu, parfois malveillant.

  </p>

  <p>

    Dans le cadre de ce lecteur audio, la faille activée concerne une <em>injection HTML</em> simple, souvent appelée <strong>XSS (Cross-Site Scripting)</strong>. Concrètement, cela signifie que si l'utilisateur saisit dans le champ d'URL une valeur contenant du code HTML ou JavaScript malicieux, ce code sera interprété et exécuté par le navigateur.

  </p>

  <p><strong>Exemple :</strong> si on entre dans le champ d'URL la valeur suivante :</p>

  <pre style="background:#222; color:#0f0; padding:10px; border-radius:5px;">

    &lt;img src=x onerror=alert('Faille exploitée!')&gt;

  </pre>

  <p>

    Le navigateur tentera de charger cette image invalide, déclenchant alors l'alerte JavaScript. Cela montre comment un utilisateur malintentionné peut insérer du code et perturber le fonctionnement normal, voire voler des données sensibles ou détourner la session.

  </p>

  <p>

    <strong>Pourquoi est-ce dangereux ?</strong>

    <ul>

      <li>Exécution de scripts malveillants pouvant voler vos données personnelles.</li>

      <li>Modification non autorisée du contenu affiché.</li>

      <li>Redirection vers des sites frauduleux ou injection de contenus malicieux.</li>

      <li>Compromission de la sécurité de l’application et de ses utilisateurs.</li>

    </ul>

  </p>

  <p>

    Dans une application professionnelle, il est impératif d'<strong>assainir toutes les entrées utilisateurs</strong> pour empêcher toute injection de code. Dans ce projet, la faille est volontairement activée pour démontrer ce risque et sensibiliser aux bonnes pratiques.

  </p>

  <p>

    Pour toute question ou suggestion, n’hésitez pas à nous <a href="mailto:support@votreentreprise.com">contacter</a>.

  </p>

</section>

<section id="securite">

  <h2>Sécurité</h2>

  <p>

    Cette application contient volontairement une faille visuelle dans la saisie de l’URL audio, permettant d’injecter du contenu HTML dans l’affichage du titre.<br>

    <strong>Cette faille est sandboxée dans une iframe isolée</strong> pour éviter toute action malveillante :  

  </p>

  <ul>

    <li>Le code injecté reste <strong>strictement contenu dans l’iframe</strong> et ne peut pas affecter la page principale.</li>

    <li>Aucune donnée n’est enregistrée ou partagée, donc le bug est <strong>temporaire et local à votre session</strong>.</li>

    <li>Le rechargement de la page remet tout à zéro, empêchant toute persistance ou propagation.</li>

    <li>Les autres utilisateurs ne sont pas affectés par cette faille.</li>

  </ul>

  <p>

    Ce choix permet d’illustrer en toute sécurité une faille XSS simple, sans risques réels pour l’utilisateur ni le système.

  </p>

</section>



</main>



<footer>

  &copy; 2025 Timothé AOUN. Tous droits réservés.

</footer>

</body>

</html>
