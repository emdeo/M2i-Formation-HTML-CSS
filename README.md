# ANTISECHE CSS

Couleurs : https://material.io/tools/color/#!/?view.left=0&view.right=0

Polices de caractères : https://www.w3schools.com/cssref/css_websafe_fonts.asp 

Icones : https://www.materialpalette.com/icons, https://material.io/tools/icons/?style=baseline

Caractères spéciaux : https://www.scriptol.fr/creation-site-web/accents-html.php



Avant HTML5 (2015), il fallait préciser dans la balise ci-dessus vers quel lien pointer pour interpréter les balises du HEAD et du BODY

RACCOURCIS
commenter = CTR + ":"
indentation = SHIFT + ALT + F

METADONNEES (celles qu'on n'affiche pas)

La balise "meta" permet : 1) d'afficher les caractères spéciaux ; 2) de présenter brièvement le document à son affichage sur un browser (Google, Yahoo, Bing...) ; 3) d'adapter la largeur du document à la largeur d'un smartphone

La balise "title" affiche le nom de la page dans l'onglet

La balise "link" permet de relier notre fichier HTML à des fichiers CSS

    <head>
        <meta charset="UTF-8"/>
        <meta name="Description" content="Une brève description de ma page ici"/>
        <meta name="viewport" content="width=device-width"/>
        <title>Kevin Dupont</title>
        <link rel="stylesheet" type="text/css" href="./assets/stylesheets/index.css" />
    </head>

EN-TETE

    <header class="maclasse1 maclasse2">

MENU avec des liens INTERNES (pointent vers des sections/divisions identifiés de ma page grâce à une ancre, par ex. #mon_id) et un lien RELATIF (ici, l'emplacement de mon fichier ("./" ) sert de point de repère)
    
    <nav class="maclasse">
        <a class="maclasse" href="#id1">Bouton 1</a>
        <a class="maclasse" href="#id2">Bouton 2</a>

        <a class="maclasse" href="./monfichier">Bouton 3</a>
    </nav>

MAIN, qui affiche du contenu additionnel (que je décide de mettre sur le côté de la page : <aside>).

Mon contenu sera divisé en SECTIONS indépendantes (par ex. "A propos de moi", "Contact"...).

L'attribut "id" construit un lien facilitant la navigation interne.

    <aside class="cartouche bg-sombre clair">
        <section id="photo">
            <img src="./dossier1/dossier2/ma_photo.png" alt="(ma photo)" class="au_centre" width="160" height="160">
        </section>

            <section id="a_propos">
                <h2 class="maclasse">
                    Mon titre
                </h2>
                <p class="maclasse">
                    Mon texte
                </p>
                <p class="maclasse">
                    Mon texte 2
                </p>

            <section id="contact">
                <h2 class="pad-m">Contact</h2>

                <!-- Liste de liens avec les balises <ul> (non ordonnée), <li> (bullets) et <ol> (ordonnée) -->
                <ul class="pad-s">
                    <!-- Liens ABSOLUS : pas de point de repère avec mon fichier actuel -->
                    <!-- Envoyer un mail en cliquant sur une image -->
                    <a href="mailto:k.dupont@yopmail.com">

                        <!-- Image en ligne dont j'ai redéfini la taille -->
                        <img src="https://ya-webdesign.com/images/email-png-logo-1.png" alt="Logo Yopmail" width=20
                            height=20>
                        M'envoyer un mail
                    </a></ul>

                <ul class="pad-s">
                    <!-- Ouvrir un nouvel onglet (target="_blank") en cliquant sur une image -->
                    <a href="https://www.google.com/search?hl=fr&q=linkedin%20kevin%20dupont" target="_blank">

                        <!-- Image en ligne dont j'ai redéfini la taille -->
                        <img src="http://www.ramphotonics.com/wp-content/uploads/2018/07/linkedin-square-white.svg"
                            alt="Logo Linkedin" width=20 height=20>
                        LinkedIn
                    </a></ul>

                <ul class="pad-s">
                    <a href="https://github.com/search?q=dupont" target="_blank">

                        <!-- Image en ligne dont j'ai redéfini la taille -->
                        <img src="https://amla26.github.io/amla-website/img/github.png" alt="Logo GitHub" width=20
                            height=20>
                        GitHub
                    </a></ul>

            </section>

            <section id="centres_d_interet">
                <h2 class="pad-m">Centres d'int&eacuter&ecirct</h2>
                <li class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </li>
                <li class="txt-justify txt-hyphens pad-s">Ideo urbs venerabilis post superbas efferatarum gentium cervices oppressas latasque
                    leges fundamenta libertatis et retinacula sempiterna velut frugi parens et prudens et dives
                    Caesaribus tamquam liberis suis regenda patrimonii iura permisit.
                </li>
                <li class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </li>
                <li class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </li>
                <li class="txt-justify txt-hyphens pad-s">Ideo urbs venerabilis post superbas efferatarum gentium cervices oppressas latasque
                    leges fundamenta libertatis et retinacula sempiterna velut frugi parens et prudens et dives
                    Caesaribus tamquam liberis suis regenda patrimonii iura permisit.
                </li>
                <li class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </li>
            </section>

        </aside>

        <!-- Balise de DIVISION : regroupe du contenu dans le même groupe -->
        <div class="principale bg-clair sombre">

            <!-- Titre -->
            <h1 id="nom">Kevin DUPONT</h1>

            <section id="competences">
                <h2 class="pad-m">Comp&eacutetences techniques</h2>
                <p class="txt-justify txt-hyphens pad-s">Nec sane haec sola pernicies orientem diversis cladibus adfligebat. Namque et Isauri,
                    quibus est usitatum saepe pacari saepeque inopinis excursibus cuncta miscere, ex latrociniis
                    occultis et raris, alente inpunitate adulescentem in peius audaciam ad bella gravia proruperunt, diu
                    quidem perduelles spiritus inrequietis motibus erigentes, hac tamen indignitate perciti vehementer,
                    ut iactitabant, quod eorum capiti quidam consortes apud Iconium Pisidiae oppidum in amphitheatrali
                    spectaculo feris praedatricibus obiecti sunt praeter morem.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Nec sane haec sola pernicies orientem diversis cladibus adfligebat. Namque et Isauri,
                    quibus est usitatum saepe pacari saepeque inopinis excursibus cuncta miscere, ex latrociniis
                    occultis et raris, alente inpunitate adulescentem in peius audaciam ad bella gravia proruperunt, diu
                    quidem perduelles spiritus inrequietis motibus erigentes, hac tamen indignitate perciti vehementer,
                    ut iactitabant, quod eorum capiti quidam consortes apud Iconium Pisidiae oppidum in amphitheatrali
                    spectaculo feris praedatricibus obiecti sunt praeter morem.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Ideo urbs venerabilis post superbas efferatarum gentium cervices oppressas latasque
                    leges fundamenta libertatis et retinacula sempiterna velut frugi parens et prudens et dives
                    Caesaribus tamquam liberis suis regenda patrimonii iura permisit.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
            </section>

            <section id="relationnel">
                <h2 class="pad-m">Relationnel</h2>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant. et cum
                    superatis difficultatibus arduis ad supercilia venissent fluvii Melanis alti et verticosi, qui pro
                    muro tuetur accolas circumfusus, augente nocte adulta terrorem quievere paulisper lucem opperientes.
                    arbitrabantur enim nullo inpediente transgressi inopino adcursu adposita quaeque vastare, sed in
                    cassum labores pertulere gravissimos.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Nec sane haec sola pernicies orientem diversis cladibus adfligebat. Namque et Isauri,
                    quibus est usitatum saepe pacari saepeque inopinis excursibus cuncta miscere, ex latrociniis
                    occultis et raris, alente inpunitate adulescentem in peius audaciam ad bella gravia proruperunt, diu
                    quidem perduelles spiritus inrequietis motibus erigentes, hac tamen indignitate perciti vehementer,
                    ut iactitabant, quod eorum capiti quidam consortes apud Iconium Pisidiae oppidum in amphitheatrali
                    spectaculo feris praedatricibus obiecti sunt praeter morem.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Ideo urbs venerabilis post superbas efferatarum gentium cervices oppressas latasque
                    leges fundamenta libertatis et retinacula sempiterna velut frugi parens et prudens et dives
                    Caesaribus tamquam liberis suis regenda patrimonii iura permisit.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
            </section>

            <section id="parcours_univ">
                <h2 class="pad-m">Parcours universitaire</h2>
                <p class="txt-justify txt-hyphens pad-s">Iis igitur est difficilius satis facere, qui se Latina scripta dicunt contemnere. in
                    quibus hoc primum est in quo admirer, cur in gravissimis rebus non delectet eos sermo patrius, cum
                    idem fabellas Latinas ad verbum e Graecis expressas non inviti legant. quis enim tam inimicus paene
                    nomini Romano est, qui Ennii Medeam aut Antiopam Pacuvii spernat aut reiciat, quod se isdem
                    Euripidis fabulis delectari dicat, Latinas litteras oderit?
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Nec sane haec sola pernicies orientem diversis cladibus adfligebat. Namque et Isauri,
                    quibus est usitatum saepe pacari saepeque inopinis excursibus cuncta miscere, ex latrociniis
                    occultis et raris, alente inpunitate adulescentem in peius audaciam ad bella gravia proruperunt, diu
                    quidem perduelles spiritus inrequietis motibus erigentes, hac tamen indignitate perciti vehementer,
                    ut iactitabant, quod eorum capiti quidam consortes apud Iconium Pisidiae oppidum in amphitheatrali
                    spectaculo feris praedatricibus obiecti sunt praeter morem.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Ideo urbs venerabilis post superbas efferatarum gentium cervices oppressas latasque
                    leges fundamenta libertatis et retinacula sempiterna velut frugi parens et prudens et dives
                    Caesaribus tamquam liberis suis regenda patrimonii iura permisit.
                </p>
                <p class="txt-justify txt-hyphens pad-s">Raptim igitur properantes ut motus sui rumores celeritate nimia praevenirent, vigore
                    corporum ac levitate confisi per flexuosas semitas ad summitates collium tardius evadebant.
                </p>
            </section>

        </div>
    </main>

    <!-- Bas de page -->
    <footer>

    </footer>
</body>

</html>


















DIMENSIONS

    width: 30%;

"vh" = viewport height (1vh = 1% de hauteur de fenêtre)

    height: 80vh;

Permet d'ajouter une barre de scroll à un block spécifique

    overflow-y: scroll;

Marges internes verticales & horizontales (déclaration pour 4 valeurs : HAUT DROIT BAS GAUCHE)
"em" = taille de la police de caractères (pratique pour définir dimensions HAUT et BAS)

    padding: 1em 1.5%;

Pour éviter de pousser la largeur d'un élément, le padding doit se soustraire à la taille de cet élément

    box-sizing: border-box;

POSITIONS

Si la propriété de position d'un élément est fixed, les propriétés top, bottom, right et left indiquent les distances entre les bords de l'élément et les bords du bloc englobant (c'est-à-dire l'ancêtre par rapport auquel l'élément est positionné). Si l'élément possède des marges, elles sont ajoutées aux décalages.

    position: fixed;

Décaler un élément de 30% de l'écran vers la droite :

    left: 30%;

Marges internes haut, droit, bas, gauche :

    padding: .5em 5em .5em 3em;

Aligner horizontalement

    display: inline-block;
    vertical-align: top;

Par défaut, chaque block a une marge de 0.25em à sa droite.
Il suffit de la fixer à -0.25em pour obtenir 2 block alignés horizontalement remplissant 30% et 70% de l'espace

    margin-right: -.25em;


Marges internes verticales & horizontales (déclaration pour 4 valeurs : HAUT DROIT BAS GAUCHE)
"em" = taille de la police de caractères (pratique pour définir dimensions HAUT et BAS)
    
    padding: 1em 1.5%;

Pour éviter de pousser la largeur d'un élément, le padding doit se soustraire à la taille de cet élément

    box-sizing: border-box;


Aligner horizontalement

    display: inline-block;
    vertical-align: top;

Par défaut, chaque block a une marge de 0.25em à sa droite.
Il suffit de la fixer à -0.25em pour obtenir 2 block alignés horizontalement remplissant 30% et 70% de l'espace

    margin-right: -.25em;

Centrer un élément horizontalement dans le block (par ex. photo perso)

    display: block;
    margin-left: auto;
    margin-right: auto;

TEXTE

Importer une langue à partir du fichier index.html dans la balise <html> (pratique, par exemple, pour insérer un tiret chaque fois que le mot est trop grand) :

    <html lang="fr">

Non surligné :

    text-decoration: none;

Mot automatiquement coupé quand il est trop grand :

    txt-align

Justifié (occupe tout l'espace horizontalement) :

    text-align:justify;

Police (Roboto est la plus utilisée sur le web) :

    font-family: Roboto, Geneva, sans-serif;

Police fine :
    
    font-weight: normal;

Ecrire un mot précis en petites majuscules :

    fichier CSS :
    .txt-maj{
        font-variant: small-caps;
    }

    fichier HTML :
    <h1 id="nom">Kevin <span class="txt-maj">dupont</span></h1>



DECLARER UN FORMULAIRE

On utilise les formulaires pour permettre au client d'envoyer des requêtes au serveur (préciser action vide par défaut). 

Méthodes disponibles : "post" (l'utilisateur peut entrer des données)

Les balises "input" sont de type "text" par défaut (on peut en utiliser d'autres : "number", "date", "color"...). Le paramètre "placeholder" donne une indication de saisie, tandis que l'attribut "required" attend qu'on entre une valeur.

    <form action="" method="post>
        <input placeholder="Votre nom" required/>
        <input type="submit"/>
    </form>



INSTALLER DE NOUVELLES LIBRAIRIES

Passer par NPM (https://nodejs.org/en/) : dans le terminal, entrer la commande "npm init" depuis le dossier stockant notre projet HTML. Le dossier "package.json" est alors automatiquement créé.

    C:\xampp\htdocs\formationHTML>npm init
    This utility will walk you through creating a package.json file.
    It only covers the most common items, and tries to guess sensible defaults.

    See `npm help json` for definitive documentation on these fields
    and exactly what they do.

    Use `npm install <pkg>` afterwards to install a package and
    save it as a dependency in the package.json file.

    Press ^C at any time to quit.
    package name: (formationhtml_manu)
    version: (1.0.0)
    description:
    entry point: (index.js)
    test command:
    git repository:
    keywords:
    author:
    license: (ISC)
    About to write to C:\xampp\htdocs\formationHTML_Manu\package.json
    
    Is this OK? (yes)
    
    C:\xampp\htdocs\formationHTML>

Importer des icônes (material-design-icons sur le site officiel www.npmjs.com)

    C:\xampp\htdocs\formationHTML>npm install material-design-icons

Importer des polices (roboto-fontface sur www.npmjs.com)

    C:\xampp\htdocs\formationHTML>npm install roboto-fontface

Enregistre automatiquement un fichier "node-modules" stockant les dépendances de "material-design-icons" et de "roboto-fontface"

Insérer une icône dans mon document

    <span class="material-icons">nom_de_l_icone</span>