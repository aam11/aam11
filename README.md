# 👋 Hi, I'm Anish Aniket Mahanta

**Atmospheric & Climate Data Specialist** at [Wind Pioneers](https://www.wind-pioneers.com) — I build the data infrastructure that wind energy decisions rest on.

Working in atmospheric and climate data since **2021**. Most of my work sits between the science and the software: reanalysis pipelines that have to be right, hazard models that have to be defensible, and tooling that turns a half-day GIS chore into a one-minute command. I care about systems that refuse to ship quietly broken data.

---

## 🔭 What I'm Building Now

**Reanalysis at scale.** ERA5 and MERRA-2 wind timeseries served from a BigQuery-backed warehouse and cloud-native zarr stores, with acquisition pipelines running from CDS and NASA GES DISC through to Google Cloud Storage.

**Correctness as a feature.** Completeness checks that raise rather than return gaps, deterministic nearest-node lookup that survives the antimeridian and the poles, dependency constraints pinned against real read failures rather than guesses.

**Hazard modelling.** Typhoon wind fields from IBTrACS best-track data, extreme wind return periods for offshore sites, and the validation work that decides whether a number is usable.

---

## 🏗️ Projects

### At Wind Pioneers

**🌬️ WindSync / Reanalysis SDK**
Python library for ERA5 and MERRA-2 wind speed and direction timeseries. Three interchangeable providers — BigQuery, GCS zarr, local netCDF — behind one API, plus a CLI and a packaged desktop app. Refuses incomplete series by default instead of silently shipping gaps. Cut reanalysis processing time by **75%** and removed **95%** of the manual handling.

**🗺️ NEWA Map Extraction**
Pulls 50 m New European Wind Atlas maps for a project area straight from a site KMZ or bounding box and writes them in the form the GIS blend expects. Minutes instead of half a day — and it checks the output rather than trusting it. The high-resolution map matters: over one Bulgarian project area the 3 km map flattened the ridges the sites actually sit on, putting **24 of 42 sites above 6.0 m/s instead of 10**.

**🌪️ Extremes Toolkit**
Extreme wind statistics for offshore sites. Holland vortex typhoon wind fields driven by IBTrACS tracks, return-period estimation via EWTS, MIS and block maxima, and a desktop runner so the analysts using it don't need a terminal.

### Personal

**🛰️ sitestack**
Stacks Earth-observation land surface temperature and precipitation timeseries for a point — twelve products across nine sources and five access mechanisms, normalised into one long-format schema with per-product zarr cubes on their native grids. Adding a new site is one YAML file.

**✈️ [meeting-airplane](https://github.com/aam11/meeting-airplane)**
macOS background app in Swift that flies a banner plane across your screen five minutes before each Outlook meeting. Written because calendar notifications are too easy to ignore.

### Earlier

**🌀 Holland Wind Field Model** — numerical cyclone/typhoon wind profiles for wind farm risk assessment.
**📦 NetCDF Maker** — R Shiny app converting raw CSV sensor data into standardised NetCDF.
**🌦️ High-Resolution Atmospheric Dataset** — **18%** forecast precision gain via deep-learning bias correction and spatial downscaling.

---

## 🧰 Toolbox

**Languages** · Python, R, SQL, MATLAB, Swift

**Climate & geospatial data** · NetCDF, GRIB, Zarr, HDF5 · ERA5, MERRA-2, ECMWF, GFS, NEWA, IBTrACS · xarray, CDO, NCO, GDAL, rasterio, QGIS, ArcGIS

**Modelling** · WRF, HYSPLIT, Holland vortex · extreme value statistics (EWTS, MIS, block maxima) · statistical downscaling · ML bias correction (LSTM, CNN) · Windographer

**Platform & engineering** · Google Cloud (BigQuery, GCS, CI/CD) · Docker, Poetry, pytest, ruff, pre-commit · REST APIs, Plumber, Swagger · Git

**Visualization** · matplotlib, Plotly, Leaflet, ggplot2

---

## 🎓 Background

### Education

**M.Sc. Atmosphere & Ocean Sciences** — Indian Institute of Technology Bhubaneswar
Dynamics, numerical modelling and ocean–atmosphere coupling; the grounding behind the hazard and reanalysis work above.

**B.Sc. Geology** — St. Xavier's College, Ranchi
Earth systems, field mapping and remote sensing — where the geospatial side started.

### Research

**Extreme rainfall variability & intraseasonal dynamics**
Characterising how monsoon rainfall extremes vary on intraseasonal timescales, and what drives the swings.

**Kalman filtering on HPC**
Sequential state estimation applied to atmospheric data, run on high-performance computing infrastructure.

### Field & Institutional Experience

**India Meteorological Department (IMD)** — national operational forecasting and observation network
**National Atmospheric Research Laboratory (NARL), Gadanki** — India's atmospheric radar and lidar facility
**Indian National Centre for Ocean Information Services (INCOIS), Hyderabad** — operational ocean forecasting and marine advisories

---

## 🌐 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/aam11)
[![X](https://img.shields.io/badge/X-black?logo=X&logoColor=white)](https://x.com/anishmahanta)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:anish.mahanta@wind-pioneers.com)

![GitHub Stats](https://github-stats-extended.vercel.app/api?username=aam11&theme=dark&show_icons=true&count_private=true)
![Top Languages](https://github-stats-extended.vercel.app/api/top-langs?username=aam11&layout=compact&theme=dark)

---

> *Scientifically sound, production-ready climate intelligence for real-world decisions.*
