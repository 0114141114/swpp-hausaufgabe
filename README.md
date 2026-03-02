# Branching Strategien

## 1. GitHub Flow

### Zentrale Charakteristik
- Sehr einfach und leichtgewichtig.  
- Nur ein Hauptbranch (`main`/`master`) und Feature-Branches.  
- Feature-Branches werden direkt in `main` gemerged, üblicherweise via Pull Request.  
- Continuous Deployment / Continuous Integration ist vorgesehen.  

### Vorteile
- Einfach zu verstehen und anzuwenden.  
- Schneller Entwicklungszyklus, gut für kleine Teams oder Projekte mit häufiger Veröffentlichung.  
- Ideal für Continuous Deployment.  

### Nachteile
- Weniger Kontrolle über Releases (kein separater Release-Branch).  
- Nicht optimal für große Teams mit komplexen Projekten.  
- Fehlende Trennung zwischen stabiler und in Entwicklung befindlicher Software.  

---

## 2. GitFlow

### Zentrale Charakteristika
- Sehr strukturiert, mehrere Branches:  
  - `main` – stabile Versionen  
  - `develop` – laufende Entwicklung  
  - `feature/*` – neue Features  
  - `release/*` – Vorbereitung eines Releases  
  - `hotfix/*` – schnelle Fehlerbehebung auf `main`  
- Geeignet für klar definierte Release-Zyklen.  

### Vorteile
- Klare Struktur und Rollback-Möglichkeiten.  
- Gut für größere Teams und Projekte mit längeren Release-Zyklen.  
- Saubere Trennung zwischen Entwicklung, Release und Hotfixes.  

### Nachteile
- Komplexer Workflow, höherer organisatorischer Aufwand.  
- Merge-Prozesse können aufwendig sein.  
- Nicht ideal für Continuous Deployment, eher für periodische Releases.  

---

## 3. GitLab Flow

### Zentrale Charakteristika
- Kombination aus GitHub Flow und GitFlow.  
- Branches nach Umgebung und Features: `main`, `production`, `staging`, `feature/*`.  
- CI/CD-Pipelines direkt integriert.  
- Flexibler Workflow: kann für Continuous Deployment oder Releases angepasst werden.  

### Vorteile
- Flexibel und an moderne CI/CD angepasst.  
- Einfacher als GitFlow, bietet trotzdem Struktur für Releases.  
- Unterstützt sowohl Feature-Entwicklung als auch stabile Produktionsversionen.  

### Nachteile
- Weniger Standardisierung, Teams müssen eigene Regeln definieren.  
- Kann für sehr kleine Projekte zu komplex sein.  
