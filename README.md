<details>

<summary>Research Context</summary>

# GBMF Phase 6 Aquaculture and Coastal Habitats Mapping for 2024
In support of the Gordon and Betty Moore Foundation's Oceans and Seafood Markets Initiative, Clark CGA has mapped an inventory of pond aquaculture and coastal habitats in top-producing countries in the global tropics using satellite imagery. The focus of this project is to monitor the rapid development of brackish shrimp aquaculture ponds and the resulting impacts on mangroves and other coastal wetlands through land change analysis. These maps are used by stakeholders worldwide to understand the spatiotemporal transition dynamics of aquaculture and coastal ecosystems to help support conservation practices and sustainability crediting in the seafood industry. 



![image](https://github.com/user-attachments/assets/45e59976-76b7-4135-99aa-d6e91d37af53)
Landsat 8 false color composite (left) of aquaculture ponds in Guayaquil, Ecuador compared to landcover map product for year 2022 (right). 



![image](https://github.com/user-attachments/assets/b3008db4-a496-4b3f-bb58-933dc12589a6)
Land change analysis for Samarinda Delta, Indonesia from 1999 - 2022 showing striking transitions from mangrove to pond aquaculture in red.



Landcover maps are produced at 15-meter resolution for 17 pantropical countries (Bangladesh, Brazil, Cambodia, China, Ecuador, El Salvador, Honduras, India, Indonesia, Malaysia, Mexico, Myanmar, Nicaragua, Philippines, Sri Lanka, Thailand, and Vietnam) for the years 1999, 2014, 2018, 2020 and 2022 (2024 in progress). The legend categories include Mangroves, Other Coastal Wetlands, Pond Aquaculture, Open Water and Other. Landcover maps for 2014 onwards are developed using pansharpened Landsat 8/9 OLI imagery, supplemented with Sentinel-1 and Sentinel-2 data where necessary (typically in cloudier regions). Landcover maps for 1999 are based on Landsat 5 ETM+ imagery. Data is provided in raster format and distributed as compressed GeoTIFF files. All data are provided using a custom equal-area global reference system that follows the specifications listed below (INSERT REF SYSTEM PARAMETERS)



![quads_global](https://github.com/user-attachments/assets/8d13df36-b913-4d59-be03-f37060034cd7)
Distribution of over 600 Landsat quads analyzed to map 17 countries.

</details>

<details>
  
<summary>Training Resources</summary>

# DIGITIZE Tutorial

## Setting Up a New Project

* Launch TerrSet by clicking on the desktop icon or searching the application in Start menu on machine. This will load the liberaGIS splash screen on your monitor.

* Once loaded, locate the TerrSet Explorer panel on the left side of the screen. Here you can revisit previous projects, create new projects, and delete projects. Users can also assign their working and resource folders in the Explorer panel. The working folder is the default location for files created within TerrSet, while the resource folders are designed to help users organize their input data. 

* Right click in the Explorer panel and click New Project (alternatively press “Insert”). Locate the ecuador folder downloaded for this tutorial and press OK. You will now see the ecuador project in your Explorer panel.

* The working folder is the folder where all new outputs will be created. Navigate to the working subfolder within the Ecuador folder using the pick list option. 

* Right click and add a resource folder and navigate to the resource subfolder within the ecuador data. This folder hosts the input data for this tutorial. 



![image](https://github.com/user-attachments/assets/c7acc56e-cbe2-4e7b-8d54-600de27948b8)



## Landsat Imagery

* Navigate to TerrSet Explorer (left side panel) and locate Files tab. Here you will see your working and resource folders. Within resource folder, click on the file labeled landsat8_false_color_composite to launch the raster image in TerrSet display. 

* User the cursor to explore the raster layer. This image is a Landsat 8 false color composite (bands 4,6,5) of a region in Ecuador where the ponds (blue/black) can be seen mosaicked across mangrove forests, which appear in a striking orange color. This will serve as a test area for this training module. 

* TerrSet comes with many useful shortcuts. To quickly zoom to the full extent of the selected raster layer, press the “Home” button. To quickly maximize the Display window on screen press “End”

* With the image selected in the composer window, press “Control+g” to launch the bounding box of the display window in Google Earth. This is an effective way to cross-reference the GIS images with Google Earth time series data to understand the landscape dynamics.



![image](https://github.com/user-attachments/assets/8d498e2e-88b4-4050-b20c-7eb9c3327f80)



## Landcover Classification

* In the resources folder you will see landcover_2024. Add this to composer display window in the following ways 
      * Right-clicking the file in Explorer and adding layer(s)
      * Dragging and dropping the image into the composer window (note this only works if the images have the same reference parameters)
      * With the layer highlighted in Explorer click Shift+Insert
      * Press “r” with composer window highlighted to launch add raster layer and locate the file using the picklist option 

* Change the palette by clicking the yellow and black checkered box in the composer window next to file name and clicking on the picklist option that pops up. Locate the file labeled Legend_Aquaculture to change the palette. This palette has been custom made for our map data to easily render the classes of interest. To view the image categories, right click on the display window and select map properties. Within the Map Properties form, select legends tab and click the radio button to make the legend 1 visible. You will now see the five categories in the display window (Mangrove, Coastal Wetlands, Pond Aquaculture, Water, Other). 

* Explore this map compared to the false color composite by toggling the layers on and off in the composer by clicking on the red check mark. As a hot key, try pressing “w” to toggle the top raster in composer on and off. To see and customize other hot keys, go to File > User Preferences > Hotkeys in the top left corner.



![image](https://github.com/user-attachments/assets/e83aa4f5-b36b-46d3-b45f-bbbfbd54f615)









</details>
