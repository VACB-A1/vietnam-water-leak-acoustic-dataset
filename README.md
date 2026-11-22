# 🔊 Vietnam Water Pipe Leak Acoustic Dataset (VWPL-AD)

> **Real-world acoustic dataset for water pipe leak detection, collected in Ho Chi Minh City, Vietnam.**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24248031.svg)](https://doi.org/10.5281/zenodo.24248031)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

---

## 📊 Dataset Overview & File Inventory

All recordings strictly adhere to the standardized acquisition parameters: **44,100 Hz, 16-bit PCM Mono, exactly 10.0 seconds per file**.

### 1. Primary Benchmark Dataset (`dataset_tuthu`)

| Category | Sub-condition / Depth | File Count | Duration | Operational Condition |
|---|---|---|---|---|
| **Leak — Night** | Buried depth 31 cm | **406** | ~67.7 min | Nighttime (quiet), pump ON, no traffic |
| **Leak — Daytime (Vehicle)** | Buried depth 32 cm | **434** | ~72.3 min | Daytime with active vehicle traffic, pump ON |
| **No Leak — Night** | 12 cm depth (`noleak_12cm`) | **125** | ~20.8 min | Baseline normal flow / static, pump OFF |
| **No Leak — Night** | 26 cm depth (`noleak_26cm`) | **177** | ~29.5 min | Baseline normal flow / static, pump OFF |
| **No Leak — Night** | Direct pipe contact (`noLeak_sat`) | **180** | ~30.0 min | Sensor coupled directly to pipe structure |
| **Subtotal (Primary Set)** | — | **1,322 files** | **~220.3 min** | **~1.11 GB** |

---

### 2. Supplementary Field Sessions (Identical 44.1 kHz Standard)

Additional real-world field sessions recorded under varying soil and acoustic conditions:

| Session | Description / Soil Condition | File Count |
|---|---|---|
| `ban_ghi_18-7_do_sau30cm_nhieu_da_va_cat` | 30 cm depth, rocky & sandy soil | **271** |
| `ban_ghi_do_sau_30cm_17-7` | 30 cm depth validation run | **42** |
| `ban_ghi_26-6` | Baseline field noise monitoring | **34** |
| `ban_ghi_20-7` | Verification recording set 1 | **10** |
| `ban_ghi_21-7` | Verification recording set 2 | **4** |
| **Subtotal (Field Sessions)** | — | **361 files** |

### 🏆 **Grand Total Qualified Dataset: 1,683 files (~280.5 minutes · ~1.41 GB)**

---

## 🎙️ Technical Specifications

| Property | Standardized Value |
|---|---|
| **Audio Format** | WAV (Uncompressed PCM) |
| **Sampling Rate** | 44,100 Hz |
| **Bit Depth** | 16-bit |
| **Channels** | Single channel (Mono) |
| **Segment Length** | 10.00 seconds per file |
| **Pipe Burial Depths** | Direct pipe contact, 12 cm, 26 cm, 30 cm, 31 cm, 32 cm |
| **Collection Location** | **Ho Chi Minh City, Vietnam** |

---

## 🛠️ Recording Hardware & IoT Node

Data was captured using a custom-engineered IoT edge node built on a Raspberry Pi architecture:
- High-sensitivity acoustic transducer / hydrophone coupled with a low-noise analog front-end.
- Synchronized ADC sampling pipeline ensuring zero sample drop across 10-second continuous windows.

> **Hardware Availability:**  
> The custom hardware sensing device, mechanical couplers, and acquisition firmware are available upon request for research groups and industrial deployments.  
> 📧 **Contact:** [langquyen235@gmail.com](mailto:langquyen235@gmail.com)

---

## 📂 Repository Structure

```
water-leak-acoustic-dataset/
├── preview/                     # 2-second WAV preview samples (public)
│   ├── leak_night/              # Sample files for night leak
│   ├── leak_daytime_vehicle/    # Sample files for daytime leak with traffic
│   └── no_leak/                 # Sample files for baseline normal state
├── preview_samples.zip          # Packaged ZIP archive of all preview samples
├── docs/                        # Technical documentation
│   ├── data_format.md
│   └── collection_protocol.md
├── LICENSE                      # CC BY-NC-ND 4.0
└── README.md
```

---

## 🖼️ Public Preview Samples

To prevent unauthorized automated scraping while allowing researchers to evaluate signal quality, **2-second preview clips** are provided in `preview/`:

| Class | Sample Files (2-second preview) |
|---|---|
| **Leak (Night)** | `leak_night_sample_01.wav` — `04.wav` |
| **Leak (Day + Vehicle)** | `leak_day_vehicle_sample_01.wav` — `04.wav` |
| **No Leak** | `no_leak_sample_01.wav` — `04.wav` |

*Download full preview archive directly: [`preview_samples.zip`](preview_samples.zip)*

---

## 💰 Full Dataset Access

The complete dataset (**1,683 files · 1.41 GB**) is distributed directly for verified research and industrial evaluations.

| Tier | Deliverables | Access Model |
|---|---|---|
| **Academic / Research** | Full WAV raw dataset + metadata labels + baseline benchmarks | On Request (Free/Academic agreement) |
| **Commercial / Industrial** | Full dataset + custom IoT recording hardware + deployment guidance | Custom Licensing |

Please email **[langquyen235@gmail.com](mailto:langquyen235@gmail.com)** with your name, institution/company, and proposed use case to request dataset access or hardware pricing.

---

## 📖 Citation

```bibtex
@dataset{nguyen2026vwpl,
  author    = {Nguyen, Tommy},
  title     = {Vietnam Water Pipe Leak Acoustic Dataset (VWPL-AD) - Preview Samples},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.24248031},
  url       = {https://doi.org/10.5281/zenodo.24248031}
}
```

---

## 📄 License

The preview samples and repository metadata are published under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)** license.
