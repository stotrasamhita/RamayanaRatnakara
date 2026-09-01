# anubandha/ — अनुबन्धाः (appendices)

`\input` by the root `ramayana-ratnakara-mulam.tex` under the book's fourth and final part.

| Folder | File | Contents |
|---|---|---|
| `valmiki-ramayanam/` | `ramayana-dhyanam.tex` | Dhyāna verse for beginning recitation of the Rāmāyaṇa. |
| | `ramayana-mangala-shloka.tex` | Maṅgala-śloka(s) for the Rāmāyaṇa. |
| `varaha-puranam/` | `varaha-puranam-dhyanam.tex` | A dhyāna verse from the Varāha Purāṇa. |
| `ramayana-mahatmyam/` | `skanda-puranam-purana-vaibhava-khanda.tex` | Rāmāyaṇa-māhātmyam, from the Purāṇa-vaibhava-khaṇḍa of the Skanda Purāṇa. |
| | `skanda-puranam-uttara-khanda.tex` | रामायणमाहात्म्यम्, from the Uttara-khaṇḍa of the Skanda Purāṇa. |

The compiled book's appendix also includes a **नामावल्यः (nāmāvalis)** section, but it isn't
sourced from a folder in this repo — the root `ramayana-ratnakara-mulam.tex` `\input`s it
directly from a **sibling repository**:

```latex
\input{../namavali-manjari/100/Rama_108}
\input{../namavali-manjari/100/Sita_108}
\input{../namavali-manjari/100/Anjaneya_108}
\input{../namavali-manjari/100/Rama_Ramarahasya_108}
\input{../namavali-manjari/100/Sita_Ramarahasya_108}
\input{../namavali-manjari/100/Anjaneya_Ramarahasya_108}
```

Six śata-nāmāvalis (Rāma, Sītā, Añjaneya, each in both its regular and *Rāma-rahasya* variants —
see [`namavali-manjari/100/README.md`](https://github.com/stotrasamhita/namavali-manjari/blob/master/100/README.md))
from the [`namavali-manjari`](https://github.com/stotrasamhita/namavali-manjari) repo. To build
the full book, clone that repo as a sibling directory of this one — see the root
[README's Building section](../README.md#building).

---

*The README.md files on this repo were generated and beautified with Claude.*
