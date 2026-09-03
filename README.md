# OPIM 5512 · Lab 1 — First Commit

**The deliverable tonight is a repo, not a notebook.** Two partners, two halves, one merge.

- **Partner A — weather** → `notebooks/Lab1_A_Weather.ipynb`, branch `dev-weather`
- **Partner B — demand** → `notebooks/Lab1_B_Demand.ipynb`, branch `dev-demand`

## What's already here (you did not have to make any of this)

```
.
├── README.md                     <- this file: the data dictionary lives here
├── REPORT.md                     <- fill this in at the end (image links already match the filenames)
├── data/clean/
│   ├── weather_hourly_hartford.csv
│   ├── weather_hourly_stamford.csv
│   └── demand_hourly.csv
├── images/                       <- your PNGs go here (drag them in)
└── notebooks/
    ├── Lab1_A_Weather.ipynb
    ├── Lab1_B_Demand.ipynb
    └── Lab1_Joint_Optional.ipynb
```

## What you add tonight

| who | file | how it gets here |
|---|---|---|
| A | `notebooks/Lab1_A_Weather.ipynb` (with your histogram) | Colab **File → Save** to branch `dev-weather` |
| A | `images/weather_line.png`, `images/weather_hist.png` | download from Colab → drag into `images/` |
| B | `notebooks/Lab1_B_Demand.ipynb` (with your histogram) | Colab **File → Save** to branch `dev-demand` |
| B | `images/demand_line.png`, `images/demand_hist.png` | download from Colab → drag into `images/` |
| both | `REPORT.md` — three sentences under the three plots | edit on `main` after both PRs merge |

## Data dictionary

### `data/clean/weather_hourly_<campus>.csv` — one row per hour, 743 rows
| column | meaning | units |
|---|---|---|
| `hour` | the hour that **begins** at this timestamp (floored from the :51 airport report) | — |
| `temp_f` | air temperature | °F |
| `dewpoint_f` | dew point | °F |
| `humidity_pct` | relative humidity | % |
| `wind_kt` | wind speed | knots |

Missing values in the raw file were the letter `M` (now blank). One hour of the month (Jul 27, 9 AM) has no report at all.

### `data/clean/demand_hourly.csv` — one row per hour, 744 rows
| column | meaning | units |
|---|---|---|
| `hour` | the hour that **begins** at this timestamp (ISO-NE *Hour Ending 01* = 00:00–01:00) | — |
| `load_mw` | total New England electricity demand | MW |

## Findings

*(Add one sentence each after your plots are in — this is where the last merge happens.)*
