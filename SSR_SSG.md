# SSR_SSG.md

1. Choisirais-tu plutôt du SSR, du SSG, ou du pré-rendu ?

   Je prendrais du SSG. Le catalogue change rarement donc on peut générer les
   pages une fois au build, et Google reçoit directement le bon HTML.

2. Si demain ce site affichait un stock en temps réel, ce choix changerait-il ?

   Pas vraiment, on garde le SSG pour la page et on récupère le stock avec un
   appel API quand la page se charge, car il change trop souvent pour être dans
   le HTML du build.
