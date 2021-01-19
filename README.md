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

Q17)