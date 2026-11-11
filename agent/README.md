# Mitt agentsystem

Fyll i instruktionerna så att någon annan kan köra och vidareutveckla agenten från en ny klon.

**Målet är ett automatiserat flöde med så lite mänsklig inblandning som möjligt.** Du bygger och konfigurerar systemet; efter start driver systemet arbetet mellan stegen. Du får använda AI för att bygga systemet. Att manuellt chatta fram dagens lösning är AI-assisterad problemlösning och uppfyller inte i sig agentspårets mål.

Börja smått och bygg vidare. Beskriv vilka steg som är automatiserade, när du behövde hjälpa till och vad du vill automatisera härnäst.

## Installera och konfigurera

- Ange verktyg, versioner, modeller och nödvändiga lokala beroenden.
- Beskriv miljövariabler med tomma eller ofarliga exempelvärden. Dela aldrig nycklar eller sessioner.
- Ange hur år, dag och del väljs. Året ska matcha `advent.json`; 2025 är vår övningsår.

## Kör och testa

Lägg in dina faktiska kommandon för installation, en agentkörning och tester. Beskriv hur man provar flödet med egna små testdata och utan att skicka svar till AoC. Förklara vilka steg som kräver mänsklig hjälp.

## Förstå och ändra flödet

- Beskriv hämta → skriva kod → testa → rätta fel och testa igen → lämna svar → publicera och var respektive steg finns i koden.
- Visa hur systemet använder återkoppling, begränsar omförsök, respekterar väntetider och stannar när det behöver hjälp.
- Lägg agentinstruktioner i `instructions/` och länka till dem här.
- Visa hur man ändrar en instruktion, byter modell och återupptar en avbruten körning.
- Beskriv ett förbättringsförslag och vad du har lärt dig av tidigare försök.

## Data och rapporter

Spara dagens lösning i `days/01/agent/`. Cachelagra AoC-material i `.private/`, respektera väntetider och stoppa återkommande fel. Kör inte loopar som gissar svar.

Rapportera använda modeller i dagens `days/NN/agent/run.json`, utan uppgiftstext, indata eller konversationer. Formatet beskrivs i `runs/README.md`. GitHub-workflowet kopplar rapporten till samma commit som lösningen.
