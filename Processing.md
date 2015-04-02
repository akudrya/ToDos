Tool | Type | Description | Data
--- | --- | --- | ---
DEM band | Geometric operations | Adding digital elevation model to make correct orthorectification and other processes | SAR & multi
Collocate |Geometric operations | collocate two spatially overlapping products | SAR & multi
Mosaic | Geometric operations | Gluing several images and cropping | SAR & multi
Reproject | Geometric operations | Create a new product with a projected Coordinate Reference System (CRS) | SAR & multi
Flip | Geometric operations | applies a flip operation to an input product and creates a new transposed output product. | SAR & multi
Ortho | Geometric operations  | Geodetic corrected with respect to the acquisition conditions such as viewing geometry, platform attitude, Earth rotation and of the relief effects (parallax) | SAR & multi
Calibration | SAR Processing | The objective of SAR calibration is to provide imagery in which the pixel values can be directly related to the radar backscatter of the scene | SAR
Object detection | Thematic -Ocean Tools | detects object such as ships on sea surface from SAR imagery | SAR
Oil spill detection | Thematic -Ocean Tools | detects dark spot such as oil spill on sea surface from SAR imagery. | SAR
Create Land Mask | Thematic -Ocean Tools | turn any pixels on land into no data value. If the "preserve land" check box is set to true then all land pixels will be preserved and all ocean pixels will be set to no data value | SAR
Wind field Estimetion | Thematic -Ocean Tools | retrieves wind speed and direction from C-band SAR imagery | SAR
Polarimetric Matrices| SAR: Polarimetric | creates the following polarimetric covariance or coherency matrices for a given full polarimetric SAR product | SAR
Polarimetric  Decomposition| SAR: Polarimetric | creates the following polarimetric covariance or coherency matrices for a given full polarimetric SAR product | SAR
Speckle Filter| SAR: Polarimetric |SAR images have inherent salt and pepper like texturing called ‘speckle’ | SAR
Orientation Angle Correction | SAR: Polarimetric | estimates the orientation angle shift θ using the circular polarization method and removes it from the polarimetric data. | SAR
Multilook | SAR Processing |  To reduce this inherent speckled appearance, several images are incoherently combined as if they corresponded to different looks of the same scene. | SAR
Cloud Probability | Pre-processing | Detecting clouds on multispectral image | multi
Sea Surface Temperature (SST) | Thematic - Water |enable the user to calculate the sea-surface temperature from (A)ATSR brightness temperatures. The SNAP implementation is explicitly open for the addition of new coefficient sets | multispectral data
SMAC | Thematic - Land |  Simplified Method for Atmospheric Correction | multispectral
NDVI | Thematic - Land | Normalized Difference Vegetation Index | multispectral
FLH / MCI |  Thematic - Land | Fluorescence Line Height and the Maximum Chlorophyll Index by exploiting the height of a measurement over a specific baseline | SAR
Clustering: k-means & EM | Image analysis - machine learning | classification of objects into different groups | SAR & multi
Principle Components |Image analysis - machine learning | generates the principal component images from a stack of co-registered detected images. The Principal Component Analysis (PCA) consists of a remapping of the information of the input co-registered images into a new set of images. The output images are scaled to prevent negative pixel values | SAR
ReplaceMetadata | Metadata processing | Replace the metadata of the first product with that of the second | Metadata of any 
TileWriter | TBD | TBD | TBD
 
