# Etichette: label printing for production reels and pallets

*Stampa delle etichette delle bobine di produzione e dei pallet*

**db** · 2000–2001 · version 1.0  
Author: **Massimo Sbarbaro** ([ORCID 0009-0006-8965-9013](https://orcid.org/0009-0006-8965-9013))

## Overview

Etichette prints the identification labels of the reels produced by a plastic-film plant. For each production order (ODL) the operator enters length, weight, colour, thickness, height, type, customer order and date, chooses the number of copies and prints the labels; the printed labels are logged. The repository contains the four variants used in the plant: the standard version, the versions for dot-matrix (needle) and laser printers, and the pallet label that reads the production-order data.

I designed and programmed this application in 2000–2001. It is published here in 2026 as part of the documented record of my software work, with a permanent DOI on Zenodo.

## Main functions

- Entry of the reel data per production order and printing of the requested number of copies (`fInserimento`, `fCopie`, `rEtichette`).
- Log of the printed labels with search by order (`fStampe`).
- Variants for needle and laser printers (`EtichetteAghi.mdb`, `EtichetteLaser.mdb`).
- Pallet label from the production-order table (`EtichettaPallet.mdb`, `sPallette`).

## Data

Tables `Generale` (label data), `Stampe` (printed labels), `codice`; in the pallet variant, `ODL` (production orders).

## Technology

db, 97 format (.mdb), forms, reports and VBA module.

## Repository contents

| Path | Content |
|---|---|
| `database/` | The database applications, emptied of all data. |
| `source/queries/` | SQL of the saved queries. |
| `docs/schema.md` | Tables and fields. |

## What is not included

The database is published **empty**: every table has been emptied, the file compacted and the unused space inside its pages overwritten with zeros, so no record of the original data survives. Logos of the organisations for which the program was built have been blanked inside the forms, and the names of organisations, people and places in captions and code have been replaced with neutral text of the same length; the application is otherwise the original file. The file is in the 1997 db format: it opens with the 1997–2010 versions of the database software; later versions must first convert it with an intermediate version.

## Related repositories

- [packing-specifications-certificates-db](https://github.com/massimosbarbaro/packing-specifications-certificates-db)
- [sheet-pack-labels-db](https://github.com/massimosbarbaro/sheet-pack-labels-db)

## How to cite

Use the citation metadata in [`CITATION.cff`](CITATION.cff) (GitHub: *Cite this repository*).

> Sbarbaro, Massimo. 2001. *Etichette: label printing for production reels and pallets*. Software (db, 2000–2001), version 1.0. GitHub. https://github.com/massimosbarbaro/production-reel-labels-db.

## License

Released under the [MIT License](LICENSE). © 2000 Massimo Sbarbaro.
