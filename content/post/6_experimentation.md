+++
title = 'Expérimentation | Hugo SSG'
date = 2024-01-25
author = "quinteirosm"
keywords = ["experimentation", "hugo", "ssg"]
cover = ""
summary = ""
+++

# Introduction

Durant le cours de LabVeilTec, on nous a demandé de rendre ces différents articles sous forme de site web utilisant un SSG afin de découvrir de nouvelles technologies. Cela m'a beaucoup intéressé car c'est un système qui permet d'avoir un site facilement gérable en terme de contenu, et cela en créant des fichiers au format MarkDown. Le SSG que j'avais choisis durant le cours était Hugo et vous pouvez en [retrouver les raisons ici.](../readme/index.html)

# Expérience [site Portfolio](https://quinteirosm.github.io/portfolio)

J'ai trouvé le sujet bien intéressant car nous devions rendre un portfolio durant le cours ProfilPro et c'est selon moi le type de projet idéal pour ce genre de framework.
De ce que j'ai pu voir sur les différents thèmes, les SSG sont souvent utilisés pour des blogs ce qui est totalement prévisible de par le format qui permet de créer des posts facilement et tout cela en ayant une infrastructure à moindre coûts.

## Résultat attendu

Je suis parti du principe qu'un portfolio est un blog, mais que les articles de blog sont remplacés par les projets qui y sont exposés. C'est pour cela que j'ai souhaité adapter le framework afin que chaque projet soit un article en markdown et qu'une boucle les génère automatiquement dans la partie expériences.

## Résultat obtenu

J'ai réussi à modifier les templates afin d'avoir un portfolio à la hauteur de mes attentes en ce qui concerne l'affichage. Cependant, étant en rush de fin de semestre, je n'ai pas eu le temps d'implémenter les projets en tant qu'articles. C'est pour cela que je me suis servi du fonctionnement de base du thème qui propose de les rentrer dans le fichier de config yaml et de les générer à partir de ce dernier.

## Améliorations futures

Pour le futur je souhaite donc mettre en place un système de cards qui serait généré à partir des articles en markdown et contiendrait la photo de cover, le titre de l'article et la description. Cela me permettrait aussi de retrieve les tags afin de pouvoir y appliquer un filtre par compétences. Cela me permettrait donc d'avoir, comme je le souhaitais, mes expériences professionnelles qui seraient auto-générées et le site serait dès lors simple à maintenir étant donner que pour ajouter ou modifier quoi que ce soit tout se passerait dans les fichiers en markdown et serait totalement dynamique.

L'option que j'envisage est aussi d'acheter un nom de domaine car [Github Pages](https://pages.github.com/) propose d'inclure un nom de domaine personalisé. Cela permettrait de passer de `quinteirosm.github.io/portfolio` à `quinteirosm.ch`. Je ne pense pas que cela importe beaucoup en ce qui concerne le recrutement mais cela rendrait tout de même le site plus professionnel.

# Conclusion

Les SSG sont en effet très pratiques pour concevoir de petits projets facilement mettables à jour. Ils permettent de s'affranchir d'une architecture lourde CMS classique avec base de données comme Wordpress par exemple. Le fait d'avoir un site statique au final permet aussi de l'héberger sur [Github Pages](https://pages.github.com/) et d'avoir dès lors aucun coût d'infrastructure car ce service est totalement gratuit. Comme tout service d'hébergement gratuit il possède des limitations mais ces dernières sont relativement larges (100GB de bande passante/mois) et ne seront sûrement jamais atteintes pour un portfolio qui est un site qui n'est pas visité très fréquemment et qui est très léger (moins de 10MB).

[Vous pouvez retrouver mon portfolio ici !](https://quinteirosm.github.io/portfolio)
