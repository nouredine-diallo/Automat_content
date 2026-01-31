# Automat_content
Automatisation Make qui transforme une video en plusieurs clip avec sous titre , des post pour adaptés aux reseaux sociaux ( twitter , linkedin ..)  et genere aussi des videos tel que quizz pour mettre en avant le contenu 

Nouredine Diallo, étudiant a Lyon 1  curieux et passionné par l'automatisation de workflows complexes. J'ai conçu ce projet pour transformer automatiquement des vidéos longues en contenus courts (TikTok/Reels) prêts à être publiés.

Le Workflow : 
Le système s'appuie sur deux scénarios Make.com qui orchestrent plusieurs services via API :

Transcription : Une vidéo déposée dans Airtable est transcrite par AssemblyAI.

IA & Analyse : GPT-4o-mini analyse le texte pour extraire les meilleures "punchlines" et définit les timestamps précis pour le découpage.

Social Media : Génération automatique de posts adaptés (LinkedIn, X, Instagram) basés sur le contenu détecté.

Rendu : Envoi des données à Creatomate pour générer le clip final au format vertical.

🛠️ Stack Technique
No-Code / Orchestration : Make (scénarios via Webhooks).

Base de données : Airtable (Dashboard de suivi).

IA : OpenAI & AssemblyAI.

Cloud & Vidéo : Google Cloud Storage, Dropbox & Creatomate API.

📁 Contenu du Repo
Alchimiste.blueprint.json : Scénario de veille et transcription.

Integration_Webhooks.blueprint.json : Logique d'analyse IA et mise à jour des données.

/scripts : Logique Python pour les traitements spécifiques car j'ai remarquer que le plan gratuit etait tres limitant donc j'ai aussi un script qui realise les montage grace a fmmeg mais c'est tres complexe 

 Apprentissages clés
Communication Inter-API : Maîtrise des flux de données via Webhooks et requêtes HTTP , Maitrise des outils No-code comme Make

Prompt Engineering : Structuration de réponses IA en JSON strict pour une intégration sans erreur.

Data Mapping : Gestion d'une base relationnelle pour le suivi de production (Status : Nouveau -> En cours -> Terminé).
