# thermokarst-lakes-alaska

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21299416.svg)](https://doi.org/10.5281/zenodo.21299416)

Analysis code and processed data for multi-sensor satellite retrieval of lake ice
phenology across ~31,000 thermokarst lakes on the Alaska North Slope (2019–2023).
Sentinel-1 SAR is classified with a random-forest model (trained on Sentinel-2 NDSI and
ERA5 temperature labels) to derive per-lake ice-on / ice-off timing, which is analysed
against latitude and lake morphometry and compared to an accumulated-degree-day model.

## Associated publication

Nguyen, A. L.\*, Lopez, C. G.\*, Melara-Valle, J., Ross, E., Bradley, A. S.,
Limbeck, M. R., Masteller, C. C., and Michaelides, R.:
*Multi-sensor satellite analysis reveals latitudinal and morphometric controls on ice
phenology across 31,000 lakes on the Alaska North Slope*
(manuscript in preparation, 2026). \
\*These authors contributed equally.

## Contents

Jupyter notebooks `01`–`06` cover ALPOD lake selection, Google Earth Engine / ERA5 data
export, the random-forest ice classifier and transition-based phenology extraction, the
spatial / morphometric analysis and accumulated-degree-day comparison, and the TROPOMI
methane companion analysis. Each notebook lists its Python dependencies and reads inputs
from Google Cloud Storage buckets hosted through Washington University in St. Louis.

## Data and code availability

Processed ice-phenology data and analysis code are archived on Zenodo (badge above,
which resolves to the persistent concept DOI). Source data: Sentinel-1/2 via Google
Earth Engine; ERA5 via the Copernicus Climate Data Store / ARCO-ERA5; ALPOD lake
polygons via the ORNL DAAC (doi:10.3334/ORNLDAAC/2399).

## License

Released under [CC-BY-4.0](LICENSE).
