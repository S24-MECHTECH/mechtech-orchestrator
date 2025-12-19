# 🧠 LENA-GEDÄCHTNIS (MECHTECH AI ORCHESTRATOR)

**Letzte Aktualisierung:** 2025-12-19
**Status:** AKTIV ✅
**Sicherheitscode:** "Lena" = Freigabe für autonome Operationen

---

## 🎯 KERN-REGELN (PERMANENT)

### 1. **STEP-BY-STEP MODUS (IMMER!)**
- Maximal 1-2 Aufgaben pro Schritt
- Warten auf "OK" oder "Lena" vor Weiterarbeit
- Keine Eigenmächtigkeit ohne Freigabe

### 2. **"LENA" AKTIVIERUNGSCODE**
- "Lena" = Autonome Operation freigegeben
- Ohne "Lena" = Nur Vorschläge, keine Ausführung
- Bei Unsicherheit = Fragen, nicht ausführen

### 3. **CURSOR = EXECUTOR (nicht Frager!)**
- Cursor arbeitet KOMPLETT AUTONOM
- Claude schreibt Tasks → Cursor macht automatisch
- KEINE Rückfragen von Cursor
- NUR Orchestrator-Entscheidungen von Claude

### 4. **GITHUB = SOURCE OF TRUTH**
- Alle wichtigen Infos in GitHub speichern
- Bei Session-Start: GitHub-Context laden
- cursor-status-live.json = Live-Kommunikation (alle 10 Sek)
- cursor-tasks.json = Aufgabenliste für Cursor

### 5. **MEMORY-CHECK ALLE 3 MINUTEN**
- Claude checkt aktiv Memory (nicht passiv warten)
- Status: "Lena Gedächtnis geladen!" + aktuelle Rules
- Cursor Posting Check durchführen
- Befehle-Ausführung überprüfen

### 6. **AUTOMATISIERUNG = PRIORITÄT #1**
- KEINE Downloads erforderlich
- KEINE Copy-Paste-Workflows
- ALLES muss automatisch laufen
- Bei manuellen Schritten → Workflow überarbeiten

---

## 📊 SUPABASE KNOWLEDGE BASE

### **3 Haupt-Tabellen:**

#### 1. **accounting_knowledge** (5GB Limit)
- Deutsche Bilanzregeln (HGB/IFRS)
- Beispielbuchungen
- Kassaabstimmung Vorlagen
- Steueropta-Szenarien
- Auto-Cleanup: Älteste zuerst

#### 2. **n8n_workflows_knowledge** (1500 beste Workflows)
- Gesammelte n8n Workflows
- Best Practices
- Error Handling Patterns
- Vektorisiert für AI-Suche

#### 3. **json_programming_knowledge**
- n8n JSON Programmierung
- KI-Integration Best Practices
- Node-Konfigurationen
- MCP Server Patterns

---

## 🚀 WORKFLOW-ARCHITEKTUR

### **MECHTECH_MERCHANT_CENTER_ADMIN**
- **Problem (gelöst):** Route by Priority blockierte 5/6 Channels
- **Lösung:** 6 Switch Nodes nach Rate Limiting
- **Target:** 92% Approval, 500 Products/Min
- **Status:** DAILY AUTO-VALIDATION via fix-workflow-auto.js

---

## 🔧 LIVE-KOMMUNIKATION

### **cursor-status-live.json** (alle 10 Sek)
- Cursor schreibt Status
- Claude liest alle 10 Sek
- REAL-TIME COMMUNICATION parallel zu Tasks

---

## 🔄 SESSION START CHECKLIST

```
☐ 1. Lena-Gedächtnis laden
☐ 2. GitHub Context prüfen
☐ 3. Cursor Status checken
☐ 4. Status: "Lena Gedächtnis geladen! ✅"
```

---

**ENDE LENA-GEDÄCHTNIS**