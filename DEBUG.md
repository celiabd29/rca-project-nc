Noussaiba - 11:49
Dans le fichier Dockerfile du backend, il y a une instruction qui essaie de copier un fichier nommé requirements.txt, mais Docker ne le trouve pas à l'endroit indiqué.

Celia — 11:56
J’ai supprimé le depends_on: backend de la configuration du service Redis. Cela résout l’erreur de cycle de dépendances qui empêchait le projet de démarrer.
