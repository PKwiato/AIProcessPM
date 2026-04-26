# AI Process PM 🚀

**Zaawansowany System Zarządzania Produktem wspomagany przez AI — Architektura Dwóch Torów**

AI Process PM to innowacyjne podejście do workflow Product Managera, które oddziela ciągłą pracę nad specyfikacją (PRD) od cyklu wytwórczego (Backlog/Sprint). System wykorzystuje 5 wyspecjalizowanych agentów AI oraz system bramek decyzyjnych "Human-in-the-Loop".

![AI Process PM Dashboard](https://raw.githubusercontent.com/PKwiato/AIProcessPM/main/og-image.png)

## 🏗️ Architektura Systemu

System opiera się na koncepcji **dwóch torów**, które komunikują się ze sobą w kluczowych punktach:

### Tor 1: PRD (Ciągły)
*   **Cel**: Utrzymanie "Żywego Dokumentu" specyfikacji.
*   **Trigger**: Nowe notatki ze spotkań, briefy, raporty UX.
*   **Rezultat**: Zawsze aktualne, zatwierdzone PRD w Confluence (v1, v2 ... v14+).
*   **Charakterystyka**: Szybkie iteracje, nieustanne wzbogacanie wiedzy o produkcie.

### Tor 2: Backlog & Sprint (Opóźniony)
*   **Cel**: Przekucie specyfikacji na konkretną pracę w Jira.
*   **Trigger**: Świadoma decyzja PM o dojrzałości PRD.
*   **Rezultat**: Gotowy Backlog, Epiki i User Stories z Acceptance Criteria (Given/When/Then).
*   **Charakterystyka**: Stabilne planowanie, minimalizacja "reworku".

---

## 🤖 Agenci AI

System wykorzystuje model agentowy do automatyzacji powtarzalnych zadań:

1.  **Agent 1: Ekstrakcja** — Zamienia surowe notatki i pliki PDF na ustrukturyzowany format JSON.
2.  **Agent 2: Analiza Diff** — Porównuje nowe dane z aktualnym PRD i znajduje różnice.
3.  **Agent 3: Patching PRD** — Aktualizuje konkretne sekcje w Confluence bez nadpisywania całego dokumentu.
4.  **Agent 4: Jira Planner** — Mapuje wymagania na strukturę Jira (Epics/Stories/AC/SP).
5.  **Agent 5: Status Reporter** — Co tydzień łączy dane z obu torów i generuje raport postępu dla stakeholderów.

---

## ⚖️ Human-in-the-Loop (Bramki PM)

Automatyzacja nie oznacza braku kontroli. W procesie zdefiniowano 5 krytycznych bramek decyzyjnych:
*   **Gate #1**: Weryfikacja ekstrakcji danych.
*   **Gate #2**: Akceptacja zmian w PRD przed publikacją nowej wersji.
*   **Gate #3**: Przegląd propozycji backlogu w Jira.
*   **Gate #4**: Finalne uruchomienie sprintu.
*   **Gate #5**: Zatwierdzenie raportu statusu przed wysyłką do zarządu.

---

## 🛠️ Stack Technologiczny

*   **Dashboard**: HTML5, Vanilla CSS, SVG (Interaktywny diagram).
*   **Orkiestracja**: n8n / Python.
*   **Modele**: Claude 3.5 Sonnet / GPT-4o.
*   **Integracje**: Jira REST API v3, Confluence Cloud API, Slack Webhooks.

---

## 🚀 Jak zacząć?

1.  Sklonuj repozytorium:
    ```bash
    git clone https://github.com/PKwiato/AIProcessPM.git
    ```
2.  Otwórz plik `ai-pm-process-v4.html` w dowolnej nowoczesnej przeglądarce.
3.  Użyj przycisku **"Uruchom Symulację"**, aby zobaczyć, jak dane przepływają przez system.
4.  Klikaj w poszczególne elementy diagramu, aby zobaczyć szczegóły implementacji, przykładowy kod i narzędzia.

---

## 📄 Licencja

Projekt udostępniony na licencji MIT. Wykorzystaj go do usprawnienia swojego workflow PM!
