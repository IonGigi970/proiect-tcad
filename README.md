# Proiect TCAD (OrCAD) – Schemă + PCB (THT)

Repo-ul conține proiectul OrCAD (Capture + PCB Editor/Allegro) în structura originală, împreună cu documentație, foi de catalog, fișiere externe (ECAD model) și exporturi pentru fabricație/asamblare.

## Structură repo
- `proiect-tcad/` – proiectul OrCAD complet (schemă, PCB, rapoarte DRC etc.)
- `foi-de-catalog/` – foi de catalog (datasheet) pentru componente
- `pdf/` – documentație + PDF-uri de tip Fab View și Assy Drawing View
- `fisiere-externe/` – pachet extern (TME/SamacSys) pentru potențiometru + instrucțiuni
- `fabricatie/` – exporturi finale: Gerber, IPC-2581, Assembly

## Fișiere principale (OrCAD)
- **Schematic (Capture):** `proiect-tcad/` (fișiere `.dsn` și `.opj`)
- **PCB (PCB Editor/Allegro):** `proiect-tcad/` (de obicei în subfolder `allegro/`, fișier `.brd`)

## Footprints / capsule (important)
### J1 – footprint custom (pitch 5 mm)
Pentru conectorul J1 a fost creată o capsulă nouă deoarece pasul pinilor este 5 mm (nu 2.54 mm). Pad-urile au fost create în Padstack Editor, iar capsula a fost definită în PCB Editor. Fișierele sunt incluse în proiect (`proiect-tcad/`).

### P1 – potențiometru (TME / SamacSys)
Pentru potențiometrul P1 a fost utilizat un model ECAD disponibil public pe pagina produsului TME (secțiunea “ECAD Model”), realizat via SamacSys. A fost necesară și adăugarea simbolului asociat în schematic, conform tutorialului PDF inclus în pachet. Pachetul este inclus în `fisiere-externe/`.

## Documentație (PDF)
În `pdf/` sunt:
- documentația proiectului
- Fab View (fabrication view)
- Assy Drawing View (assembly drawing)

## Fabricație / Asamblare
Exporturile finale sunt în `fabricatie/`:
- `fabricatie/gerber/` – Gerber + drill (Excellon / NC Drill)
- `fabricatie/ipc2581/` – IPC-2581 (dacă există)
- `fabricatie/assembly/` – fișiere pentru asamblare (dacă există)

## Recomandare
Păstrează structura din `proiect-tcad/` neschimbată pentru a evita probleme de paths în OrCAD.

## Licență
MIT – vezi `LICENSE`.
