
[![Eurostat online]( https://img.shields.io/badge/everything_starts_here-go_social!-blue.png?style=plastic)]( https://github.com/eurostat/) 
eurostat@github
===============

### About

[_Eurostat_](http://ec.europa.eu/eurostat) is the statistical office of the European Union. We provide high quality statistics for Europe.

Contributions are welcome: we invite your participation through collaboration, issues, and pull requests!

### Contents

#### Data handling and processing ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5)

* [PING](https://github.com/eurostat/PING): Library of macro/function utilities developed (`R`/`SAS`/`Stata`) for the implementation of statistical processes in production environments (_note_: other components of the GSBPM model are also identified in this resource).
* [JGiscoTools](https://github.com/eurostat/JGiscoTools): Manipulation of geographical and statistical data in `Java`, with a focus on _Eurostat_ data.
* [EuroGen](https://github.com/eurostat/EuroGen): Some automated map generalisation processes and software for the production of European geographical datasets.
* [GridMaker](https://github.com/eurostat/GridMaker): `Java` tool to produce grid geometries for European statistics.
* [searoute](https://github.com/eurostat/searoute): Computation of shortest maritime routes between ports in `Java`.
* [RegionSimplify](https://github.com/eurostat/RegionSimplify): `Java` tool to simplify vector geographical datasets representing tesselations, such as administrative regions, land cover areas. 

#### Data integration and record linkage ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5.1)

* [ICW](https://github.com/eurostat/ICW): Codes (`R`) for experimental statistics on household income, consumption and wealth (see _statistics-coded_).

#### Statistical data editing ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5.3 | 5.4)

* [flagr](https://github.com/eurostat/flagr): A simple `R` package to derive flag for aggregates.

#### Data validation and transformation ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5.3 | 5.4 | 5.5 | 5.6 | 5.7)

* [VTL](https://github.com/eurostat/VTL): interpreter of `VTL` (Validation and Transformation Language) provided together with the sandbox user interface.

#### Estimation ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5.6 | 5.7)

* [econowcast](https://github.com/eurostat/econowcast): Experimental tools (`R`) for Big Data econometrics nowcasting and early estimates.
*  [ecobackcast](https://github.com/eurostat/ecobackcast): Experimental tools (`R`) for back-casting principal European Economic Indicators. 
* [quantile](https://github.com/eurostat/quantile): Agnostic (re)implementations (`R`/`SAS`/`Python`/`C`) of common quantile estimation algorithms.

#### Time series ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 5.6 | 5.7)

* [prophet](https://github.com/eurostat/prophet): Applying (in `Python`) Facebook Prophet model for forecasting Eurostat monthly indicators.

#### Statistical disclosure control ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 6.4)

* [confly](https://github.com/eurostat/confly): Implementation (`SAS`) of disclosure control methods for microdata confidentiality on the fly.

#### Visualisation ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 7.2)

* [d3.sunburst](https://github.com/eurostat/d3.sunburst): Reusable function (`Javascript`) to easily create sunburst visualizations based on `D3.js`.
* [EurostatVisu](https://github.com/eurostat/EurostatVisu): Web visualisations (`Javascript`) of _Eurostat_ data.
* [d3.examples](https://github.com/eurostat/d3.examples): Applying `d3.js` framework for handling and exploring (`Javascript`/`Python`) _Eurostat_ data and metadata.
* [EuroGridVisualizer](https://github.com/eurostat/EuroGridVisualizer): `Three.js` visualization for gridded statistics. 
* [regl-map-animation](https://github.com/eurostat/regl-map-animation): Configurable `WebGL` animation showing a map transitioning into a chart.

#### Dissemination products ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 7.2)

* [statistics-coded](https://github.com/eurostat/statistics-coded): Catalogue of resources (`R`/`Python`/`SQL`/`SAS`/`Stata`/...) to reproduce the results of _Eurostat_ Stastistics Explained articles.
* [dff](https://github.com/eurostat/dff): Promoting the use of a publically available scanner data set in price index research and for capacity building (`R`/`SAS`).

#### Access to official statistics ([GSBPM](https://statswiki.unece.org/display/GSBPM/Generic+Statistical+Business+Process+Model) 7.4)

* [PRost](https://github.com/eurostat/PRost): Self-contained platform to access and handle _Eurostat_ data in `Python` and `R`.
* [java4eurostat](https://github.com/eurostat/java4eurostat): `Java` library for multi-dimensional data manipulation and easy access to _Eurostat_ data.
* [eurostat.js](https://github.com/eurostat/eurostat.js): `Javascript` libraries for _Eurostat_ data users and web developers.
* [Nuts2json](https://github.com/eurostat/Nuts2json): Various versions of _Eurostat_ NUTS dataset as `JSON` formats, for web mapping.
* [pyrostat](https://github.com/eurostat/pyrostat): `Python` API to _Eurostat_ online database.
* [happyGISCO](https://github.com/eurostat/happyGISCO): Simple microservice (`Python` API) built on top of _Eurostat_ GISCO web-services.
 * [restatapi](https://github.com/eurostat/restatapi): An `R` package to search and retrieve data from _Eurostat_ online database.
* [PowerBI-connector](https://github.com/eurostat/PowerBI-connector): `PowerBI` custom connector for _Eurostat_ API.

#### Working together

* [udoxy](https://github.com/eurostat/udoxy): Guidelines and script (`bash`) for generic standalone code documentation.
* [beamslide](https://github.com/eurostat/beamslide): _Eurostat_ layout style/template for `LaTeX` beamer presentation.
* [bibestat](https://github.com/eurostat/bibestat): _Eurostat_ bibliographical footprint, references and citations. 

### Note

Any resemblance between this page and the [awesome list of statistical software packages](https://github.com/SNStatComp/awesome-official-statistics-software) is certainly not coincidental. 

### Disclaimer

This repository contains open resources developed in-house and with partners.

The sole responsibility for the content of this webpage lies with the authors. It does not necessarily reflect the opinion of the European Union. Neither _Eurostat_ nor the European Commission are responsible for any use that may be made of the information contained therein.

Access to and use of the contents of this website is at the user‘s own risk. Damage and warranty claims arising from missing or incorrect resources are excluded. The authors bear no responsibility or liability for damage of any kind, also for indirect or consequential damages resulting from access to or use of the contents of this website.

