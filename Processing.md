Tool | Type | Description | Data
--- | --- | --- | ---
DEM band | Geometric operations | Adding digital elevation model to make correct orthorectification and other processes | SAR & multi
Collocate |Geometric operations | collocate two spatially overlapping products | SAR & multi
Mosaic | Geometric operations | Gluing several images and cropping | SAR & multi
Reproject | Geometric operations | Create a new product with a projected Coordinate Reference System (CRS) | SAR & multi
Flip | Geometric operations | applies a flip operation to an input product and creates a new transposed output product. | SAR & multi
Ortho | Geometric operations  | geodetic corrected with respect to the acquisition conditions such as viewing geometry, platform attitude, Earth rotation and of the relief effects (parallax).| SAR & multi

##### Utilities:
Data Conversion
Mask 
Resampling
BandsMaths 
BandSelect 
Image-Filter 
Import-Vector
ReplaceMetadata
TileWriter 

##### SAR Processing
Coregistration | SAR Processing | 
Interferometric
Ocean Tools
Polarimetric
Radiometric
Speckle Filtering
Multilook 

##### Optical Processing
Pre-processing Cloud Probability - for MERIS Level 1b only
Sea Surface Temperature (SST) | Thematic - Water |enable the user to calculate the sea-surface temperature from (A)ATSR brightness temperatures. The SNAP implementation is explicitly open for the addition of new coefficient sets | multispectral data
SMAC | Thematic - Land |  Simplified Method for Atmospheric Correction | multispectral
NDVI | Thematic - Land | Normalized Difference Vegetation Index | multispectral
FLH / MCI |  Thematic - Land | Fluorescence Line Height and the Maximum Chlorophyll Index by exploiting the height of a measurement over a specific baseline | SAR

##### Image Analysis
Clustering: k-means & EM | Image analysis - machine learning | classification of objects into different groups | SAR or multispectral
Texture analysis 
Change detection
Principle Components
Speckle Divergence
