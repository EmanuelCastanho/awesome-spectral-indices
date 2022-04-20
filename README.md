<p align="center">
  <a href="https://github.com/davemlz/awesome-spectral-indices"><img src="https://raw.githubusercontent.com/davemlz/awesome-spectral-indices/main/docs/_static/asi.png" alt="Awesome Spectral Indices"></a>
</p>
<p align="center">
    <em>A ready-to-use curated list of Spectral Indices for Remote Sensing applications.</em>
</p>
<p align="center">
<a href="https://github.com/sindresorhus/awesome" target="_blank">
    <img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg" alt="Awesome">
</a>
<a href="https://github.com/davemlz/awesome-ee-spectral-indices/blob/main/output/spectral-indices-dict.json" target="_blank">
    <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/davemlz/5e9f08fa6a45d9d486e29d9d85ad5c84/raw/spectral.json" alt="Awesome Spectral Indices">
</a>
<a href="https://share.streamlit.io/davemlz/espectro/main/espectro.py" target="_blank">
    <img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg" alt="Streamlit">
</a>
<a href="https://github.com/davemlz/awesome-ee-spectral-indices/actions/workflows/tests.yml" target="_blank">
    <img src="https://github.com/davemlz/awesome-ee-spectral-indices/actions/workflows/tests.yml/badge.svg" alt="Tests">
</a>
<a href="https://awesome-ee-spectral-indices.readthedocs.io/en/latest/?badge=latest" target="_blank">
    <img src="https://readthedocs.org/projects/awesome-ee-spectral-indices/badge/?version=latest" alt="Documentation">
</a>
<a href="https://zenodo.org/badge/latestdoi/355720108"><img src="https://zenodo.org/badge/355720108.svg" alt="DOI"></a>
<a href="https://github.com/sponsors/davemlz" target="_blank">
    <img src="https://img.shields.io/badge/GitHub%20Sponsors-Donate-ff69b4.svg" alt="GitHub Sponsors">
</a>
<a href="https://www.buymeacoffee.com/davemlz" target="_blank">
    <img src="https://img.shields.io/badge/Buy%20me%20a%20coffee-Donate-ff69b4.svg" alt="Buy me a coffee">
</a>
<a href="https://ko-fi.com/davemlz" target="_blank">
    <img src="https://img.shields.io/badge/kofi-Donate-ff69b4.svg" alt="Ko-fi">
</a>
<a href="https://twitter.com/dmlmont" target="_blank">
    <img src="https://img.shields.io/twitter/follow/dmlmont?style=social" alt="Twitter">
</a>
<a href="https://github.com/psf/black" target="_blank">
    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
</a>
</p>

---

**GitHub**: <a href="https://github.com/davemlz/awesome-ee-spectral-indices" target="_blank">github.com/davemlz/awesome-ee-spectral-indices</a>

**Documentation**: <a href="https://awesome-ee-spectral-indices.readthedocs.io/" target="_blank">awesome-ee-spectral-indices.readthedocs.io</a>

**Python Package**: <a href="https://github.com/davemlz/spyndex" target="_blank">github.com/davemlz/spyndex</a>

**Streamlit App**: <a href="https://github.com/davemlz/espectro" target="_blank">github.com/davemlz/espectro</a>

**Google Earth Engine**: <a href="https://github.com/davemlz/eemont" target="_blank">github.com/davemlz/eemont</a> (Python), <a href="https://github.com/davemlz/spectral" target="_blank">github.com/davemlz/spectral</a> (JavaScript) and <a href="https://github.com/r-earthengine/rgeeExtra" target="_blank">github.com/r-earthengine/rgeeExtra</a> (R)

---

<style>
    table {
        width: 100%;
    }
</style>

# Spectral Indices

Spectral Indices are widely used in the Remote Sensing community. This repository keeps track of classical as well as novel spectral indices for different Remote Sensing applications. All spectral indices in the repository are curated and can be used in different environments and programming languages. 
You can check the [curated list of spectral indices here](https://github.com/davemlz/awesome-ee-spectral-indices/blob/main/output/spectral-indices-table.csv), and if you want to use it in your environment, it is available in [CSV](https://raw.githubusercontent.com/davemlz/awesome-ee-spectral-indices/main/output/spectral-indices-table.csv) and [JSON](https://raw.githubusercontent.com/davemlz/awesome-ee-spectral-indices/main/output/spectral-indices-dict.json).

## Attributes

All spectral indices follow a standard. Each item of the list has the following attributes:

- `short_name`: Short name of the index (e.g. `"NDWI"`).
- `long_name`: Long name of the index (e.g. `"Normalized Difference Water Index"`).
- `formula`: Expression/formula of the index (e.g. `"(G - N)/(G + N)"`).
- `bands`: List of required bands/parameters for the index computation (e.g. `["N","G"]`).
- `reference`: Link to the index reference/paper/doi (e.g. `"https://doi.org/10.1080/01431169608948714"`).
- `type`: Type/application of the index (e.g. `"water"`).
- `date_of_addition`: Date of addition to the list (e.g. `"2021-04-07"`).
- `contributor`: GitHub user link of the contributor (e.g. `"https://github.com/davemlz"`).

## Expressions

The formula of the index is presented as a string/expression (e.g. `"(N - R)/(N + R)"`) that can be easily evaluated. The parameters used in the expression for each index follow this standard:

<table>

<tr>

<th> Description </th>
<th> Standard </th>
<th> Sentinel-1 </th>
<th> Sentinel-2 </th>
<th> Landsat-89 </th>
<th> Landsat-457 </th>
<th> MODIS </th>

</tr>

<tr>

<td>Aerosols</td>
<td>A</td>
<td></td>
<td>B1</td>
<td>B1</td>
<td></td>
<td></td>

</tr>

<tr>

<td>Blue</td>
<td>B</td>
<td></td>
<td>B2</td>
<td>B2</td>
<td>B1</td>
<td>B3</td>

</tr>

<tr>

<td>Green</td>
<td>G</td>
<td></td>
<td>B3</td>
<td>B3</td>
<td>B2</td>
<td>B4</td>

</tr>

<tr>

<td>Red</td>
<td>R</td>
<td></td>
<td>B4</td>
<td>B4</td>
<td>B3</td>
<td>B1</td>

</tr>

<tr>

<td>Red Edge 1</td>
<td>RE1</td>
<td></td>
<td>B5</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Red Edge 2</td>
<td>RE2</td>
<td></td>
<td>B6</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Red Edge 3</td>
<td>RE3</td>
<td></td>
<td>B7</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>NIR</td>
<td>N</td>
<td></td>
<td>B8</td>
<td>B5</td>
<td>B4</td>
<td>B2</td>

</tr>

<tr>

<td>NIR 2</td>
<td>N2</td>
<td></td>
<td>B8A</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>SWIR 1</td>
<td>S1</td>
<td></td>
<td>B11</td>
<td>B6</td>
<td>B5</td>
<td>B6</td>

</tr>

<tr>

<td>SWIR 2</td>
<td>S2</td>
<td></td>
<td>B12</td>
<td>B7</td>
<td>B7</td>
<td>B7</td>

</tr>

<tr>

<td>Thermal 1</td>
<td>T1</td>
<td></td>
<td></td>
<td>B10</td>
<td>B6</td>
<td></td>

</tr>

<tr>

<td>Thermal 2</td>
<td>T2</td>
<td></td>
<td></td>
<td>B11</td>
<td></td>
<td></td>

</tr>

<tr>

<td>Backscattering Coefficient HV</td>
<td>HV</td>
<td>HV</td>
<td></td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Backscattering Coefficient VH</td>
<td>VH</td>
<td>VH</td>
<td></td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Backscattering Coefficient HH</td>
<td>HH</td>
<td>HH</td>
<td></td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Backscattering Coefficient VV</td>
<td>VV</td>
<td>VV</td>
<td></td>
<td></td>
<td></td>
<td></td>

</tr>

</table>

Additional index parameters also follow a standard:

- `g`: Gain factor (e.g. Used for EVI).
- `L`: Canopy background adjustment (e.g. Used for SAVI and EVI).
- `C1`: Coefficient 1 for the aerosol resistance term (e.g. Used for EVI).
- `C2`: Coefficient 2 for the aerosol resistance term (e.g. Used for EVI).
- `cexp`: Exponent used for OCVI.
- `nexp`: Exponent used for GDVI.
- `alpha`: Weighting coefficient used for WDRVI, BWDRVI and NDPI.
- `beta`: Calibration parameter used for NDSIns.
- `gamma`: Weighting coefficient used for ARVI.
- `omega`: Weighting coefficient used for MBWI.
- `sla`: Soil line slope.
- `slb`: Soil line intercept.
- `PAR`: Photosynthetically Active Radiation.
- `k`: Slope parameter by soil used for NIRvH2.
- `lambdaN`: NIR wavelength used for NIRvH2 and NDGI.
- `lambdaR`: Red wavelength used for NIRvH2 and NDGI.
- `lambdaG`: Green wavelength used for NDGI.

The kernel indices are constructed using a special type of parameters:

- `kAB`: Kernel of bands/parameters `A` and `B` (e.g. `kNR` means `k(N,R)`, where `k` is the kernel function).
- `p`: Kernel degree (used for the polynomial kernel).
- `c`: Free parameter that trades off the influence of higher-order versus lower-order terms (used for the polynomial kernel).

# Call for Indices! :rotating_light:

Researchers that have published (or aim to publish) their novel spectral indices are encouraged to add them to this repository! The list of spectral indices is used as a source for different resources that allow spectral indices computation in different environments (such as Python and Google Earth Engine). To add an index, please follow the [Contribution Guidelines](https://awesome-ee-spectral-indices.readthedocs.io/en/latest/contributing.html).

In the same line, if you know an spectral index that is not included in this repository, you are encouraged to add it! Please follow the [Contribution Guidelines](https://awesome-ee-spectral-indices.readthedocs.io/en/latest/contributing.html) in order to add it.

And one more thing: If you see an error in one or several indices, please report it or update the index (indices) by following the [Contribution Guidelines](https://awesome-ee-spectral-indices.readthedocs.io/en/latest/contributing.html)!

There is no deadline. The repository is continuously updated!

# Used by

## JavaScript

- [spectral](https://github.com/davemlz/spectral): Awesome Spectral Indices for the Google Earth Engine JavaScript API (Code Editor).

## Python

- [eemont](https://github.com/davemlz/eemont): A Python package that extends Google Earth Engine.
- [eeExtra](https://github.com/r-earthengine/ee_extra): A Python package that unifies the Google Earth Engine ecosystem.
- [Espectro](https://github.com/davemlz/espectro): The Awesome Spectral Indices Streamlit App.
- [spyndex](https://github.com/davemlz/spyndex): Awesome Spectral Indices in Python.

## R

- [rgeeExtra](https://github.com/r-earthengine/rgeeExtra): High-level functions to process spatial and simple Earth Engine objects.

# Spectral Indices by Type


## Vegetation


### A
<table><tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00190-0" target="_blank">AFRI1600</a>: Aerosol Free Vegetation Index (1600 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00190-0" target="_blank">AFRI2100</a>: Aerosol Free Vegetation Index (2100 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1562/0031-8655(2001)074%3C0038:OPANEO%3E2.0.CO;2" target="_blank">ARI</a>: Anthocyanin Reflectance Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1562/0031-8655(2001)074%3C0038:OPANEO%3E2.0.CO;2" target="_blank">ARI2</a>: Anthocyanin Reflectance Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/36.134076" target="_blank">ARVI</a>: Atmospherically Resistant Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(91)90009-U" target="_blank">ATSAVI</a>: Adjusted Transformed Soil-Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.465.8749&rep=rep1&type=pdf" target="_blank">AVI</a>: Advanced Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### B
<table><tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(87)90088-5" target="_blank">BCC</a>: Blue Chromatic Coordinate.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S1672-6308(07)60027-4" target="_blank">BNDVI</a>: Blue Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2135/cropsci2007.01.0031" target="_blank">BWDRVI</a>: Blue Wide Dynamic Range Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### C
<table><tr><td width="50%"><a href="https://doi.org/10.1078/0176-1617-00887" target="_blank">CIG</a>: Chlorophyll Index Green.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1078/0176-1617-00887" target="_blank">CIRE</a>: Chlorophyll Index Red Edge.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.cabdirect.org/cabdirect/abstract/20073176046" target="_blank">CVI</a>: Chlorophyll Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### D
<table><tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(94)00114-3" target="_blank">DVI</a>: Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2019.03.028" target="_blank">DVIplus</a>: Difference Vegetation Index Plus.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### E
<table><tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(96)00112-5" target="_blank">EVI</a>: Enhanced Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2008.06.006" target="_blank">EVI2</a>: Two-Band Enhanced Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.13031/2013.27838" target="_blank">ExG</a>: Excess Green Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.compag.2008.03.009" target="_blank">ExGR</a>: ExG - ExR Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1117/12.336896" target="_blank">ExR</a>: Excess Red Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### F
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2020.111676" target="_blank">FCVI</a>: Fluorescence Correction Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### G
<table><tr><td width="50%"><a href="https://www.indexdatabase.de/db/i-single.php?id=363" target="_blank">GARI</a>: Green Atmospherically Resistant Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.indexdatabase.de/db/i-single.php?id=186" target="_blank">GBNDVI</a>: Green-Blue Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(87)90088-5" target="_blank">GCC</a>: Green Chromatic Coordinate.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs6021211" target="_blank">GDVI</a>: Generalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1007/bf00031911" target="_blank">GEMI</a>: Global Environment Monitoring Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1080/10106040108542184" target="_blank">GLI</a>: Green Leaf Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(96)80284-7" target="_blank">GM1</a>: Gitelson and Merzlyak Index 1.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(96)80284-7" target="_blank">GM2</a>: Gitelson and Merzlyak Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(96)00072-7" target="_blank">GNDVI</a>: Green Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">GOSAVI</a>: Green Optimized Soil Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.indexdatabase.de/db/i-single.php?id=185" target="_blank">GRNDVI</a>: Green-Red Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">GRVI</a>: Green Ratio Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">GSAVI</a>: Green Soil Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00037-8" target="_blank">GVMI</a>: Global Vegetation Moisture Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### I
<table><tr><td width="50%"><a href="https://www.jipb.net/EN/abstract/abstract23925.shtml" target="_blank">IAVI</a>: New Atmospherically Resistant Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1006/anbo.1997.0544" target="_blank">IKAW</a>: Kawashima Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(90)90085-Z" target="_blank">IPVI</a>: Infrared Percentage Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.isprsjprs.2013.04.007" target="_blank">IRECI</a>: Inverted Red-Edge Chlorophyll Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### M
<table><tr><td width="50%"><a href="http://dx.doi.org/10.1016/S0034-4257(00)00113-9" target="_blank">MCARI</a>: Modified Chlorophyll Absorption in Reflectance Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2003.12.013" target="_blank">MCARI1</a>: Modified Chlorophyll Absorption in Reflectance Index 1.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2003.12.013" target="_blank">MCARI2</a>: Modified Chlorophyll Absorption in Reflectance Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.agrformet.2008.03.005" target="_blank">MCARI705</a>: Modified Chlorophyll Absorption in Reflectance Index (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(00)00113-9" target="_blank">MCARIOSAVI</a>: MCARI/OSAVI Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.agrformet.2008.03.005" target="_blank">MCARIOSAVI705</a>: MCARI/OSAVI Ratio (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2015.02.012" target="_blank">MGRVI</a>: Modified Green Red Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/014311697216810" target="_blank">MNDVI</a>: Modified Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/TGRS.2003.812910" target="_blank">MNLI</a>: Modified Non-Linear Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/s20185055" target="_blank">MRBVI</a>: Modified Red Blue Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(94)90134-1" target="_blank">MSAVI</a>: Modified Soil-Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(89)90046-1" target="_blank">MSI</a>: Moisture Stress Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/07038992.1996.10855178" target="_blank">MSR</a>: Modified Simple Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.agrformet.2008.03.005" target="_blank">MSR705</a>: Modified Simple Ratio (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/0143116042000274015" target="_blank">MTCI</a>: MERIS Terrestrial Chlorophyll Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2003.12.013" target="_blank">MTVI1</a>: Modified Triangular Vegetation Index 1.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2003.12.013" target="_blank">MTVI2</a>: Modified Triangular Vegetation Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00010-X" target="_blank">mND705</a>: Modified Normalized Difference (705, 750 and 445 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00010-X" target="_blank">mSR705</a>: Modified Simple Ratio (705 and 445 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### N
<table><tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00010-X" target="_blank">ND705</a>: Normalized Difference (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1029/2006GL029127" target="_blank">NDDI</a>: Normalized Difference Drought Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2019.03.028" target="_blank">NDGI</a>: Normalized Difference Greenness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.asprs.org/wp-content/uploads/pers/1983journal/jan/1983_jan_77-83.pdf" target="_blank">NDII</a>: Normalized Difference Infrared Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00318-2" target="_blank">NDMI</a>: Normalized Difference Moisture Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2017.04.031" target="_blank">NDPI</a>: Normalized Difference Phenology Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/1011-1344(93)06963-4" target="_blank">NDREI</a>: Normalized Difference Red Edge Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://ntrs.nasa.gov/citations/19740022614" target="_blank">NDVI</a>: Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(11)81633-0" target="_blank">NDVI705</a>: Normalized Difference Vegetation Index (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2016.06.016" target="_blank">NDYI</a>: Normalized Difference Yellowness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(79)90013-0" target="_blank">NGRDI</a>: Normalized Green Red Difference Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.1602244" target="_blank">NIRv</a>: Near-Infrared Reflectance of Vegetation.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2021.112723" target="_blank">NIRvH2</a>: Hyperspectral Near-Infrared Reflectance of Vegetation.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2021.112763" target="_blank">NIRvP</a>: Near-Infrared Reflectance of Vegetation and Incoming PAR.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/02757259409532252" target="_blank">NLI</a>: Non-Linear Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1029/2007GL031021" target="_blank">NMDI</a>: Normalized Multi-band Drought Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs13010105" target="_blank">NRFIg</a>: Normalized Rapeseed Flowering Index Green.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs13010105" target="_blank">NRFIr</a>: Normalized Rapeseed Flowering Index Red.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">NormG</a>: Normalized Green.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">NormNIR</a>: Normalized NIR.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj2004.0314" target="_blank">NormR</a>: Normalized Red.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### O
<table><tr><td width="50%"><a href="http://dx.doi.org/10.1007/s11119-008-9075-z" target="_blank">OCVI</a>: Optimized Chlorophyll Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(95)00186-7" target="_blank">OSAVI</a>: Optimized Soil-Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### P
<table><tr><td width="50%"><a href="https://doi.org/10.1034/j.1399-3054.1999.106119.x" target="_blank">PSRI</a>: Plant Senescing Reflectance Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### R
<table><tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(87)90088-5" target="_blank">RCC</a>: Red Chromatic Coordinate.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(94)00114-3" target="_blank">RDVI</a>: Renormalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/s18030868" target="_blank">REDSI</a>: Red-Edge Disease Stress Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(11)81633-0" target="_blank">RENDVI</a>: Red Edge Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2015.02.012" target="_blank">RGBVI</a>: Red Green Blue Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2014.03.018" target="_blank">RGRI</a>: Red-Green Ratio Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.documentation.ird.fr/hor/fdi:34390" target="_blank">RI</a>: Redness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2134/agronj1968.00021962006000060016x" target="_blank">RVI</a>: Ratio Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### S
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.isprsjprs.2013.04.007" target="_blank">S2REP</a>: Sentinel-2 Red-Edge Position.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/36.134076" target="_blank">SARVI</a>: Soil Adjusted and Atmospherically Resistant Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(88)90106-X" target="_blank">SAVI</a>: Soil-Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431169008955053" target="_blank">SAVI2</a>: Soil-Adjusted Vegetation Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.465.8749&rep=rep1&type=pdf" target="_blank">SI</a>: Shadow Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://eurekamag.com/research/009/395/009395053.php" target="_blank">SIPI</a>: Structure Insensitive Pigment Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.2307/1936256" target="_blank">SR</a>: Simple Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431169308904370" target="_blank">SR2</a>: Simple Ratio (800 and 550 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(98)00046-7" target="_blank">SR3</a>: Simple Ratio (860, 550 and 708 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(11)81633-0" target="_blank">SR555</a>: Simple Ratio (555 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0176-1617(11)81633-0" target="_blank">SR705</a>: Simple Ratio (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/s19040904" target="_blank">SeLI</a>: Sentinel-2 LAI Green Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### T
<table><tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00018-4" target="_blank">TCARI</a>: Transformed Chlorophyll Absorption in Reflectance Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(02)00018-4" target="_blank">TCARIOSAVI</a>: TCARI/OSAVI Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.agrformet.2008.03.005" target="_blank">TCARIOSAVI705</a>: TCARI/OSAVI Ratio (705 and 750 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1109/TGRS.2007.904836" target="_blank">TCI</a>: Triangular Chlorophyll Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.2002.1026867" target="_blank">TDVI</a>: Transformed Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1016/j.jag.2012.07.020" target="_blank">TGI</a>: Triangular Greenness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs12152359" target="_blank">TRRVI</a>: Transformed Red Range Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.1989.576128" target="_blank">TSAVI</a>: Transformed Soil-Adjusted Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs12010016" target="_blank">TTVI</a>: Transformed Triangular Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://ntrs.nasa.gov/citations/19740022614" target="_blank">TVI</a>: Transformed Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1016/S0034-4257(00)00197-8" target="_blank">TriVI</a>: Triangular Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### V
<table><tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00289-9" target="_blank">VARI</a>: Visible Atmospherically Resistant Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00289-9" target="_blank">VARI700</a>: Visible Atmospherically Resistant Index (700 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00289-9" target="_blank">VI700</a>: Vegetation Index (700 nm).</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/S0034-4257(01)00289-9" target="_blank">VIG</a>: Vegetation Index Green.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### W
<table><tr><td width="50%"><a href="https://doi.org/10.1078/0176-1617-01176" target="_blank">WDRVI</a>: Wide Dynamic Range Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/0034-4257(89)90076-X" target="_blank">WDVI</a>: Weighted Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

## Water


### A
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2013.08.029" target="_blank">AWEInsh</a>: Automated Water Extraction Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2013.08.029" target="_blank">AWEIsh</a>: Automated Water Extraction Index with Shadows Elimination.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### L
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2003.11.008" target="_blank">LSWI</a>: Land Surface Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### M
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2018.01.018" target="_blank">MBWI</a>: Multi-Band Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs71215805" target="_blank">MLSWI26</a>: Modified Land Surface Water Index (MODIS Bands 2 and 6).</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs71215805" target="_blank">MLSWI27</a>: Modified Land Surface Water Index (MODIS Bands 2 and 7).</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160600589179" target="_blank">MNDWI</a>: Modified Normalized Difference Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs10101643" target="_blank">MuWIR</a>: Revised Multi-Spectral Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### N
<table><tr><td width="50%"><a href="https://doi.org/10.1007/978-3-662-45737-5_51" target="_blank">NDVIMNDWI</a>: NDVI-MNDWI Model.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431169608948714" target="_blank">NDWI</a>: Normalized Difference Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/w12051339" target="_blank">NDWIns</a>: Normalized Difference Water Index with no Snow Cover and Glaciers.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.11873/j.issn.1004-0323.2009.2.167" target="_blank">NWI</a>: New Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### S
<table><tr><td width="50%"><a href="https://doi.org/10.3390/w13121647" target="_blank">S2WI</a>: Sentinel-2 Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://eoscience.esa.int/landtraining2017/files/posters/MILCZAREK.pdf" target="_blank">SWM</a>: Sentinel Water Mask.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### W
<table><tr><td width="50%"><a href="https://doi.org/10.3390/rs11182186" target="_blank">WI1</a>: Water Index 1.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs11182186" target="_blank">WI2</a>: Water Index 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/GEOINFORMATICS.2010.5567762" target="_blank">WRI</a>: Water Ratio Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

## Burn


### B
<table><tr><td width="50%"><a href="https://digital.csic.es/bitstream/10261/6426/1/Martin_Isabel_Serie_Geografica.pdf" target="_blank">BAI</a>: Burned Area Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.foreco.2006.08.248" target="_blank">BAIM</a>: Burned Area Index adapted to MODIS.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/ecrs-2-05177" target="_blank">BAIS2</a>: Burned Area Index for Sentinel 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### C
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2005.04.014" target="_blank">CSI</a>: Char Soil Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160600954704" target="_blank">CSIT</a>: Char Soil Index Thermal.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
</table>

### M
<table><tr><td width="50%"><a href="https://doi.org/10.1080/01431160110053185" target="_blank">MIRBI</a>: Mid-Infrared Burn Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### N
<table><tr><td width="50%"><a href="https://doi.org/10.3133/ofr0211" target="_blank">NBR</a>: Normalized Burn Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.usgs.gov/core-science-systems/nli/landsat/landsat-normalized-burn-ratio-2" target="_blank">NBR2</a>: Normalized Burn Ratio 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160500239008" target="_blank">NBRT1</a>: Normalized Burn Ratio Thermal 1.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160500239008" target="_blank">NBRT2</a>: Normalized Burn Ratio Thermal 2.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160500239008" target="_blank">NBRT3</a>: Normalized Burn Ratio Thermal 3.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160600954704" target="_blank">NDVIT</a>: Normalized Difference Vegetation Index Thermal.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
</table>

### S
<table><tr><td width="50%"><a href="https://doi.org/10.1080/01431160600954704" target="_blank">SAVIT</a>: Soil-Adjusted Vegetation Index Thermal.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
</table>

### V
<table><tr><td width="50%"><a href="https://doi.org/10.1080/01431160500239008" target="_blank">VI6T</a>: VI6T Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
</table>

## Snow


### N
<table><tr><td width="50%"><a href="https://doi.org/10.3390/rs13142777" target="_blank">NBSIMS</a>: Non-Binary Snow Index for Multi-Component Surfaces.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160802385459" target="_blank">NDGlaI</a>: Normalized Difference Glacier Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.1994.399618" target="_blank">NDSI</a>: Normalized Difference Snow Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160802385459" target="_blank">NDSII</a>: Normalized Difference Snow Ice Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/w12051339" target="_blank">NDSInw</a>: Normalized Difference Snow Index with no Water.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/01431160119766" target="_blank">NDSaII</a>: Normalized Difference Snow and Ice Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### S
<table><tr><td width="50%"><a href="https://doi.org/10.3178/jjshwr.12.28" target="_blank">S3</a>: S3 Snow Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/rs11232774" target="_blank">SWI</a>: Snow Water Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

## Urban


### B
<table><tr><td width="50%"><a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.465.8749&rep=rep1&type=pdf" target="_blank">BI</a>: Bare Soil Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1080/10106049.2018.1497094" target="_blank">BLFEI</a>: Built-Up Land Features Extraction Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.2005.1525743" target="_blank">BaI</a>: Bareness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### D
<table><tr><td width="50%"><a href="https://doi.org/10.3390/land7030081" target="_blank">DBI</a>: Dry Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/land7030081" target="_blank">DBSI</a>: Dry Bareness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### E
<table><tr><td width="50%"><a href="https://doi.org/10.3390/rs4102957" target="_blank">EBBI</a>: Enhanced Built-Up and Bareness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2022.102703" target="_blank">EMBI</a>: Enhanced Modified Bare Soil Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### I
<table><tr><td width="50%"><a href="https://doi.org/10.1080/01431160802039957" target="_blank">IBI</a>: Index-Based Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### M
<table><tr><td width="50%"><a href="https://doi.org/10.3390/land10030231" target="_blank">MBI</a>: Modified Bare Soil Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### N
<table><tr><td width="50%"><a href="https://doi.org/10.3390/rs9030249" target="_blank">NBLI</a>: Normalized Difference Bare Land Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://hdl.handle.net/1959.11/29500" target="_blank">NBUI</a>: New Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="http://dx.doi.org/10.1080/01431160304987" target="_blank">NDBI</a>: Normalized Difference Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.2005.1526319" target="_blank">NDBaI</a>: Normalized Difference Bareness Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.14358/PERS.76.5.557" target="_blank">NDISIb</a>: Normalized Difference Impervious Surface Index Blue.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.14358/PERS.76.5.557" target="_blank">NDISIg</a>: Normalized Difference Impervious Surface Index Green.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.14358/PERS.76.5.557" target="_blank">NDISImndwi</a>: Normalized Difference Impervious Surface Index with MNDWI.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.14358/PERS.76.5.557" target="_blank">NDISIndwi</a>: Normalized Difference Impervious Surface Index with NDWI.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.14358/PERS.76.5.557" target="_blank">NDISIr</a>: Normalized Difference Impervious Surface Index Red.</td><td width="50%"> <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.jag.2015.02.010" target="_blank">NDSoI</a>: Normalized Difference Soil Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://www.semanticscholar.org/paper/Using-WorldView-2-Vis-NIR-MSI-Imagery-to-Support-Wolf/5e5063ccc4ee76b56b721c866e871d47a77f9fb4" target="_blank">NHFD</a>: Non-Homogeneous Feature Difference.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/land10030231" target="_blank">NSDS</a>: Normalized Shortwave Infrared Difference Soil-Moisture.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### P
<table><tr><td width="50%"><a href="https://doi.org/10.3390/rs10101521" target="_blank">PISI</a>: Perpendicular Impervious Surface Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### U
<table><tr><td width="50%"><a href="https://www.isprs.org/proceedings/XXXI/congress/part7/321_XXXI-part7.pdf" target="_blank">UI</a>: Urban Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

### V
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.ecolind.2015.03.037" target="_blank">VgNIRBI</a>: Visible Green-Based Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1016/j.ecolind.2015.03.037" target="_blank">VrNIRBI</a>: Visible Red-Based Built-Up Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

## Kernel


### K
<table><tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.abc7447" target="_blank">kEVI</a>: Kernel Enhanced Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.abc7447" target="_blank">kIPVI</a>: Kernel Infrared Percentage Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.abc7447" target="_blank">kNDVI</a>: Kernel Normalized Difference Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.abc7447" target="_blank">kRVI</a>: Kernel Ratio Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1126/sciadv.abc7447" target="_blank">kVARI</a>: Kernel Visible Atmospherically Resistant Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-MODIS-green?style=flat-square" alt="MODIS">  <img src="https://img.shields.io/badge/-Landsat%20457-blueviolet?style=flat-square" alt="Landsat-457">  <img src="https://img.shields.io/badge/-Landsat%2089-blue?style=flat-square" alt="Landsat-89">  <img src="https://img.shields.io/badge/-Sentinel%202-red?style=flat-square" alt="Sentinel-2"> </td></tr>
</table>

## Radar


### D
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2018.09.003" target="_blank">DPDD</a>: Dual-Pol Diagonal Distance.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://www.tandfonline.com/doi/abs/10.5589/m12-043" target="_blank">DpRVIHH</a>: Dual-Polarized Radar Vegetation Index HH.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/app9040655" target="_blank">DpRVIVV</a>: Dual-Polarized Radar Vegetation Index VV.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
</table>

### N
<table><tr><td width="50%"><a href="https://www.isprs.org/proceedings/XXXVII/congress/4_pdf/267.pdf" target="_blank">NDPolI</a>: Normalized Difference Polarization Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
</table>

### Q
<table><tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS.2001.976856" target="_blank">QpRVI</a>: Quad-Polarized Radar Vegetation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
</table>

### R
<table><tr><td width="50%"><a href="https://doi.org/10.5194/bg-9-179-2012" target="_blank">RFDI</a>: Radar Forest Degradation Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
</table>

### V
<table><tr><td width="50%"><a href="https://doi.org/10.1016/j.rse.2018.09.003" target="_blank">VDDPI</a>: Vertical Dual De-Polarization Index.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/app9040655" target="_blank">VHVVD</a>: VH-VV Difference.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS47720.2021.9554099" target="_blank">VHVVP</a>: VH-VV Product.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS47720.2021.9554099" target="_blank">VHVVR</a>: VH-VV Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS47720.2021.9554099" target="_blank">VVVHD</a>: VV-VH Difference.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.3390/app9040655" target="_blank">VVVHR</a>: VV-VH Ratio.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
<tr><td width="50%"><a href="https://doi.org/10.1109/IGARSS47720.2021.9554099" target="_blank">VVVHS</a>: VV-VH Sum.</td><td width="50%"> <img src="https://img.shields.io/badge/-Sentinel%201-gray?style=flat-square" alt="Sentinel-1"> </td></tr>
</table>

# List

Check the full list of spectral indices with their formulas [here](https://github.com/davemlz/awesome-ee-spectral-indices/blob/main/output/spectral-indices-table.csv).

# Download Raw Files

You can download or clone the repository:

```
git clone https://github.com/davemlz/awesome-ee-spectral-indices.git
```

Or you can download the single files here (right-click > Save link as...):

- JSON: [Raw list](https://raw.githubusercontent.com/davemlz/awesome-ee-spectral-indices/main/output/spectral-indices-dict.json)
- CSV: [Raw list](https://raw.githubusercontent.com/davemlz/awesome-ee-spectral-indices/main/output/spectral-indices-table.csv)

# Credits

- [César Aybar](https://github.com/csaybar): The formidable [pydantic](https://github.com/samuelcolvin/pydantic/) expert and creator of [rgee](https://github.com/r-spatial/rgee).
