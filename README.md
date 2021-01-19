TD Déployer une application web

Q4) $vercel -v

Q5) $vercel init angular

Q6) $cd angular
    $vercel

Q7) $vercel ls td-deploy-vercel

Q8) $vercel logs td-deploy-vercel.vercel.app

Q9) $vercel inspect td-deploy-vercel.vercel.app
    La commande permet d'avoir des informations sur le projet et son déploiement
    On retrouve des infos général comme son id et son nom, ses fichiers et les routes.

Q10) Une variable d'environnement permet de configurer un ou des paramètres d'un outil déployé sous vercel

Q11) $vercel env add plain VAR_PROD production

Q12) $vercel env ls

Q13) Ces variables sont chiffrées dans les variables d'environnement, comme par exemple pour les mots de passe.
     
Q15) $vercel secret add variable2_secret ceciestuntest35
     $vercel env add secret secret_n_2 production
     On affecte ensuite variable2_secret à secret_n_2

Q16) Les 3 environnements sont Production, Preview et Development.
     Ces 3 environnement permettent de développer sans affecter le rendu finale, ou de faire des test sans créer de problèmes sur notre code.
     Ici, on peut développer sur l'environnement Development, faire des test sur Preview et le rendu final sur Production par exemple.

Q18) https://td-deploy-vercel.yanneb.vercel.app/

Q19) Une pull request permet à un utilisateur de modifier une partie d'un code sans modifier la branche master.
     Lorsqu'il va pousser son code, cela va créer une autre branche qui pourra être merge avec le master si toutes les personnes utilisant un projet sont d'accord par exemple

     Ajout d'un fichier pour faire un changement sur la nouvelle branche.
     Pull request sur la nouvelle branche. Voir screen "Question19.png" dans le dossier.
     
     Vercel déploie la pull request dans un environnement Preview.

Q20) Une fois le merge réalisé, Vercel déploie cette pull request sur l'environnement Production

Q21) L'environnement de production correspond à la branche Master/main
     Avec des pull request on peut avoir des versions temporaires de notre projet et on peut tester le bon fonctionnement de celui-ci avant de déployer l'application.
     On peut donc faire différents tests avant de le merge sur le master.
     Workflow : On crée une nouvelle branche pour la feature -> On développe ce qu'on a à faire -> On push sur Github -> On fait un pull request -> On test dans l'environnement preview
                -> On merge si c'est validé 

Q22) Le severless permet à un développeur de créer et exécuter sans gérer de serveurs. Tout est géré via un cloud. Il faut envoyer le code dans des conteneurs pour avoir l'application. 
     Les ressources serveurs sont allouées dynamiquement.
     Cela permet au développeur de se concentrer sur son travail.