# 🔥 FireMind ERP   
**AI-powered Fire Safety Compliance Assistant for Public Buildings (ERP)**  
**Assistant intelligent de conformité en sécurité incendie pour les Établissements Recevant du Public (ERP)**  


---

🚨 Problème
** La conformité incendie dans les ERP est **:

Complexe et chronophage
Sujette aux erreurs humaines
Basée sur des textes réglementaires lourds
Difficile à standardiser
Coûteuse pour les bureaux d’études et organismes de contrôle
Les professionnels passent des heures à vérifier manuellement les règles et rédiger des rapports.

---

## 💡 Solution    

FireMind ERP est une plateforme intelligente qui automatise et simplifie la conformité incendie.

Elle permet :

Génération automatique des règles applicables

Checklists d’audit intelligentes

Détection des non‑conformités

Génération de rapports PDF professionnels

Mode inspection mobile

Gestion documentaire centralisée

Alertes pour les échéances et inspections

---

⚙️ Fonctionnalités principales
🧠 Moteur intelligent de réglementation
Entrées : type ERP, surface, effectif, étages

Sorties : règles applicables

Matching dynamique (JSON/YAML)

Détection automatique des non‑conformités

📋 Système d’audit intelligent
Checklist générée dynamiquement

Validation conforme / non conforme

Observations, commentaires, photos

Mode inspection hors‑ligne

📄 Génération automatique de rapports
Rapports PDF professionnels

Compatibles commissions de sécurité

Score de conformité, photos, recommandations

📸 Mode inspection terrain
Interface mobile

Capture photo & annotation

Marquage rapide des non‑conformités

📊 Tableau de bord de conformité
Score global

Priorisation des risques

Gestion multi‑sites

🏗️ Architecture technique
Stack technique
Backend : Python (FastAPI) ou C# (.NET)

Frontend : React ou Blazor

Base de données : PostgreSQL

Autres : OCR, générateur PDF, reconnaissance d’images 

Architecture système 
┌──────────────────────┐       ┌──────────────────────────┐
│      Frontend        │ <---->│        API Backend        │
│ React / Blazor       │       │ FastAPI / .NET            │
└──────────────────────┘       └───────────────┬───────────┘
                                                │
                                      ┌─────────▼───────────┐
                                      │     PostgreSQL DB    │
                                      └──────────────────────┘

🗂️ Modèle de données
Tables principales 


Table	                      Description
Users	                      Rôles : admin, contrôleur, manager
Establishments	            Type ERP, surface, effectif, adresse
Audits	                    Checklist, conformité, photos, observations
Documents	                  Plans, certificats, rapports
Alerts	                    Échéances, inspections, renouvellement matériel


Exemple de règle 

{
  "erp_type": "M",
  "rules": [
    { "id": "EXT-01", "description": "1 extincteur pour 200 m²", "severity": "medium" },
    { "id": "EVAC-03", "description": "2 issues de secours minimum", "severity": "high" }
  ]
}

🧪 Exemple d’audit 

ERP : Type M – Surface 850 m² – 2 niveaux
Conformité globale : 78%

❌ Non‑conformités détectées :
- EXT‑01 : Nombre d’extincteurs insuffisant
- SIG‑04 : Absence de signalisation lumineuse

📄 Rapport généré : report_erp_m_2024_03.pdf


🚀 Feuille de route
MVP
Moteur de règles

Système d’audit

Génération PDF

Prochaines étapes
Gestion multi‑projets

Mode inspection mobile

Conformité assistée par IA

Reconnaissance d’images

Carte interactive d’évacuation

🎯 Utilisateurs cibles
Bureaux d’études

Consultants en sécurité incendie

Architectes

Organismes de contrôle (SOCOTEC, Bureau Veritas, APAVE…) 

🧭 Installation (dev)
Backend 
pip install -r requirements.txt
uvicorn app.main:app --reload

Frontend
npm install
npm run dev

📌 Vision
Devenir l’assistant IA de référence pour la conformité incendie des ERP en Europe. 

## 👤 Auteur 

Hamza Abdelli  
Embedded Systems & Autonomous Engineering Student  
Étudiant ingénieur en systèmes embarqués et autonomes  
[LinkedIn](https://www.linkedin.com/in/hamza-abdelli-/)  

---
