En simpel og pålidelig strømforsynings-switch baseret på **LTC4359 ideal diode controller**. Enheden sørger automatisk for fejlfri overgang mellem primær strøm og backup-strømkilde, når hovedstrømmen forsvinder.

Perfekt til udstyr, der kræver kontinuerlig drift – f.eks. routere, overvågningskameraer eller netværksudstyr.

## Egenskaber

- **Automatisk failover** mellem hoved- og backup-strømforsyning
- **LTC4359-baseret**: effektiv og tabsfri styring af strømretningen
- **Ingen mikrokontroller eller software**
- **Indgangsspænding (Vin):** 9–80 V DC
- **Maks. udgangsstrøm:** 8,5 A (begrænset af stik og printbaner)
- **Passiv og vedligeholdelsesfri**
- **Kompakt design med 3D-printet kabinet**

## Indhold

- `schematic/BackupPowerSwitch.pdf` – Skematisk diagram
- `case/` – STL-filer til 3D-printet kabinet
- `README.md` – Denne dokumentation

## Funktion

- To separate strømindgange: én til hovedforsyning og én til backup.
- LTC4359 styrer en MOSFET, som fungerer som en ideel diode med lavt spændingsfald.
- Ved spændingsudfald på hovedforsyningen, skifter systemet automatisk og øjeblikkeligt til backup.
- Når hovedforsyningen vender tilbage, overtager den igen automatisk.

## Anvendelsesområder

- UPS-løsninger til små enheder
- Netværksudstyr og routere
- IoT-installationer
- Kamera- og alarmsystemer

![](https://github.com/gert-lauritsen/BackupPowerSwicht/blob/main/Doc/Screenshot%202025-07-01%20133015.png)

![](https://github.com/gert-lauritsen/BackupPowerSwicht/blob/main/Doc/03994fa3-5506-4035-915d-3ff298bebc68.png)

## Bemærkninger og begrænsninger

- Sørg for tilstrækkelig køling ved kontinuerlig belastning over 3 A
- Udgangen er ikke galvanisk adskilt – kun egnet til DC-spændinger
- LTC4359 prioriterer automatisk den højeste indgangsspænding – ikke egnet til aktiv paralleldrift
