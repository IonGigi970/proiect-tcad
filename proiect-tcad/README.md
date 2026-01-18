# proiect-tcad/

Acest folder conține proiectul OrCAD în structura originală (așa cum a fost lucrat).

## Ce găsești aici
- Fișiere de proiect pentru **OrCAD Capture** (schematic) – ex: `.dsn`, `.opj`
- Fișierul plăcii pentru **PCB Editor/Allegro** – ex: `.brd` (de obicei într-un subfolder `allegro/`)
- Alte fișiere generate pe parcurs (ex: DRC, netlist/wirelist, rapoarte)

## Cum se deschide proiectul
1. Deschide OrCAD Capture și încarcă proiectul (fișierul `.opj` sau `.dsn`).
2. Deschide OrCAD PCB Editor/Allegro și încarcă placa (`.brd`).

## Footprints / librării
- **J1 (conector):** footprint/capsulă custom, pitch 5 mm (realizată cu Padstack Editor + PCB Editor).
- **P1 (potențiometru):** model ECAD de la TME/SamacSys + simbol asociat în schematic.
  - Pachetul descărcat (cu tutorial) este în `../fisiere-externe/`.

## Notă despre mutări
E recomandat să nu schimbi structura acestui folder decât dacă actualizezi și căile (paths) folosite de OrCAD.
