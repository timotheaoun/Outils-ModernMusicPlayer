# À propos de Modern Music Player

_Un outil en ligne pour apprendre facilement le HTML en injectant du code dans un input, vous pouvez bien entendu l'utiliser comme lecteur de musique..._

---

## Ma mission

Bonjour, je me présente, je suis **Timothé AOUN**.  
Je suis passionné par la programmation, les maths et le hacking. Mon objectif est de pouvoir transmettre mon savoir et surtout d'apprendre en vous apprenant, me former en vous formant. C'est pourquoi, sur mon [Site web](https://timotheaoun.github.io/), vous retrouverez plusieurs projets mathématiques et informatiques qui valent le coup d'œil.  
**Modern Music Player** est un outil que j'ai initialement conçu à usage personnel, pour écouter de la musique. Remarquant une énorme faille HTML, j'ai décidé de la conserver et d'en faire un "bac à sable", dans lequel vous pouvez injecter du code.

---

## Ce que vous trouverez ici

Cette page _« À propos »_ a pour but de vous expliquer en détail les subtilités de l'outil :

- **Interface Moderne :** design épuré, thème sombre, simplement pour être agréable
- **Performance :** chargement rapide, navigation fluide
- **Apprentissage :** Apprenez à maîtriser le HTML et ses failles à travers un exemple d'outil en ligne très facilement détournable. Je précise que je fais cela dans un but éducatif, l'objectif n'étant pas de vous apprendre le hacking, mais de vous faire cerner son mode de fonctionnement afin que vous puissiez mieux vous en protéger.

---

## Fonctionnement

Une **faille** en informatique désigne une vulnérabilité ou une faiblesse dans un logiciel ou une application qui peut être exploitée par un attaquant pour causer un comportement non prévu, parfois malveillant.

Dans le cadre de ce lecteur audio, la faille activée concerne une _injection HTML_ simple, souvent appelée **XSS (Cross-Site Scripting)**. Concrètement, cela signifie que si l'utilisateur saisit dans le champ d'URL une valeur contenant du code HTML ou JavaScript malicieux, ce code sera interprété et exécuté par le navigateur.

**Exemple :**

```html
<img src=x onerror=alert('Faille exploitée!')> 
