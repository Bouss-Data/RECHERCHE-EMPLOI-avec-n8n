# RECHERCHE-EMPLOI-avec-n8n
c'est un assistant virtuel sur-mesure pour automatiser une recherche d'emploi ciblée, qualitative et chronophage sans avoir à parcourir manuellement des dizaines de sites chaque jour (LinkedIn, sites de l'ONU, Banque Mondiale, GIZ, etc.).


Ce workflow n8n (intitulé "RECHERCHE EMPLOI") sert d'agent d'intelligence artificielle automatisé pour effectuer une veille sur les opportunités professionnelles récentes (Emploi, Stage, Consultance).


1. Objectif principal
Il recherche de manière autonome des offres publiées au cours des 30 derniers jours qui ciblent principalement le Gabon, l'Afrique centrale, ou des postes en télétravail ouverts aux candidats africains.

2. Secteurs et Domaines ciblés
L'agent filtre rigoureusement les annonces pour ne retenir que celles liées à :

Data et IA : Data Science, Big Data, Machine Learning, Data Analyst, Automatisation.

SIG & Géomatique : Cartographie, Télédétection, analyse spatiale.

Environnement & Climat : Gestion forestière, biodiversité, REDD+, finance climat.

Développement communautaire & Recherche appliquée : Inclusion sociale, études d’impact environnemental, suivi écologique.

3. Fonctionnement technique du Workflow
Le processus est entièrement automatisé à l'aide de 4 nœuds interconnectés :

Schedule Trigger (Déclencheur horaire) : Planifie et lance l'automatisation de manière récurrente (configuré à 11h).

AI Agent (L'Agent IA) : Le cœur du workflow. Il est programmé avec des instructions système très strictes (gestion des doublons, vérification des dates, interdiction de s'appuyer sur des rumeurs, formatage spécifique).

Google Gemini Chat Model (Le modèle LLM) : Utilise l'IA gemini-3.5-flash pour analyser les données textuelles, faire les recherches et synthétiser les offres sous forme de fiches de lecture standardisées.

Send a message in Gmail (Outil d'envoi) : Une fois la veille terminée, l'agent utilise cet outil pour envoyer directement le rapport finalisé par email à l'adresse indiquée.
