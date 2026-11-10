# REFLEXION.md

1. `robots.txt` empêche-t-il, à lui seul, le duplicate content entre
   `/produits?tri=prix` et `/produits?tri=prix-asc` ? Pourquoi ?

   Non, robots.txt bloque juste l'exploration des pages. Les deux URLs peuvent
   quand même être indexées, donc le duplicate content reste.

2. Pourquoi la balise canonique est-elle l'outil adapté ici, plutôt que
   `robots.txt` ou une meta `noindex` ?

   La canonique dit à Google quelle version garder quand plusieurs URLs
   affichent la même chose. Avec noindex on retirerait la page de Google alors
   qu'on veut qu'une des deux reste.

3. Si demain `/admin` existe sur ce site et ne doit jamais être exploré par
   Google, quelle ligne ajoutes-tu dans `robots.txt` ?

   `Disallow: /admin`
