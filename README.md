# swiss-gazetteer-matching
Annotated data for the [GIR'17](http://www.geo.uzh.ch/~rsp/gir17/) short paper _Gazetteer matching for natural features in Switzerland_.

## Annotated data
Feature IDs from **[GeoNames](http://www.geonames.org/)** are listed alongside matched feature IDs from **SwissNames3D**. The IDs are from the respective datasets, which can be obtained at the following links:
 - GeoNames: http://download.geonames.org/export/dump/ then choose `CH.zip` for the Switzerland data
 - SwissNames3D: https://shop.swisstopo.admin.ch/en/products/landscape/names3D

Please review yourself the terms of use of the data from GeoNames and SwissNames3D! The GeoNames data dump used for our annotation is from July 20th 2017, but it is updated frequently so there may be changes. 

The annotated data is presented as a CSV file in the `data` folder. The data is tab-separated and contains GeoNames IDs and SwissNames IDs. SwissNames IDs contain curly brackets, i.e. `{...}`, as part of the IDs. The main match for each GeoNames feature (`geonameid`) is listed under `swissnamesid` and any additional matches are listed under `extra_matches`, with each extra match separated by a semi-colon `;`.

A simple example to read this file is shown as a Jupyter notebook, 'Example_file_read.ipynb' in the main directory. See the following link for more info about  [Jupyter notebooks](http://jupyter-notebook.readthedocs.io/en/latest/notebook.html).

## Further info
Our annotation process is described in our short paper and was presented at the [2017 Geographic Information Retrieval workshop](http://www.geo.uzh.ch/~rsp/gir17/) in Heidelberg. Please have a look at the paper for further info and kindly cite our paper if you find the annotated data useful for your own work:

Elise Acheson, Julia Villette, Michele Volpi, and Ross S. Purves. 2017. Gazetteer matching for natural features in Switzerland. In _GIR’17: 11th Workshop on Geographic Information Retrieval, November 30-December 1, 2017, Heidelberg, Germany_. ACM, New York, NY, USA, 2 pages. https://doi.org/10.1145/3155902.3155913
