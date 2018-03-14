Synopsis du projet transverse 
 
Objectif du projet 
 
Le projet, dans sa finalité, consiste à créer une application et un logiciel qui permettent respectivement de prendre en photo et de scanner un document au format manuscrit comme une prise de note et de le transcrire en format numérique en conservant la mise en page. La quantité de travail étant trop élevé pour un semestre, nous avons, si l’état du projet le permet, l’ambition de le prolonger en 3ème année.

Nous ciblons les milieux scolaire et professionnels qui utilisent encore l’écriture manuscrite. Des élèves ont souvent des prises de note brouillonnes, qui méritent une mise en page propre pour faciliter l’apprentissage. Une formule mathématique, par exemple, n’est ni simple ni rapide à écrire dans un logiciel de traitement de texte. Par ailleurs, les professeurs trouveront leur intérêt dans l’élaboration de cours s’ils ne sont pas à l’aise avec un clavier d’ordinateur ou s’il serait plus rapide de les écrire à la main. L’application rendrait aussi plus simple la correction de certaines copies (par exemple, des programmes écrits à la main en les faisant tourner sur ordinateur directement, ou tout simplement des textes à trous). On pourrait encore prolonger ces applications à la copie de vieux documents manuscrits (pour les musés ou archives)  

Eléments de conception 
 
L’application fonctionnera par divers algorithmes de reconnaissance d’image à base de neurones artificiels. Le principe sera de reconnaitre les types d’objets manuscrits présents sur une page (texte brut, formules, schémas, tableaux…) pris en photo, puis de les traiter séparément. Pour chaque type, le programme rescindera les éléments successivement (texte brut 
→
 mot 
→
 lettre, formule 
→
 opérateur/fonction 
→
 chiffres/lettres…par exemple). Pour cela nous entrainerons nos algorithmes sur une base d’exemples déjà disponibles ou créés par nous-même ou bien acquis par l’expérience. Nous utiliserons le langage python qui nous propose divers outils open source additionnels simplifiant la programmation de réseaux de neurones tels que TensorFlow ou Keras. 
Par la diversité des fonctionnalités et leur difficulté, nous nous concentrerons sur une d’entre elles : la reconnaissance de formules mathématiques. Celle-ci nécessite la détection de chiffres, de lettres isolées (alphabet latin et alphabet grec) mais aussi de tous les symboles mathématiques classiques (+, =, /, *, <). Ce sera l’objectif principal à atteindre pour ce semestre. S’il est atteint, nous nous focaliserons sur les autres, comme la reconnaissance de texte brut, de tableaux ou de schémas. 
 
 
 
 
 
Feuille de route 
 
Nous commencerons par la reconnaissance d’écriture mathématiques. Nous procéderons en plusieurs étapes : 

Initiation à python et aux bibliothèques additionnelles (TensorFlow, Keras) 

Premier réseau de neurones reconnaissant les chiffres 

Un réseau pour les lettres 

Un réseau pour les caractères mathématiques (ponctuation, opérateur, symboles, fonctions, fractions, matrices…) 

Concevoir un algo de séparation d’objet 

Lier le tout et enregistrer le résultat dans un logiciel de traitement de texte (probablement Latex). 
 
