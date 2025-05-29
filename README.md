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

<summary>Quad List</summary>



PLACEHOLDER
		

  
</details>



<details>
  
<summary>Training Resources</summary>

### Tutorial 1: Where do I store this data?

<details>

 
<summary>Folder Setup</summary>
 
1) Create a folder labelled 'Moore' in your PCs data drive.

![image](https://github.com/user-attachments/assets/f4114424-de88-45c0-a2e0-ca8516849279)


2) The Moore folder should contain GIS_Files (downloaded from canvas) and a folder for each country we're working in.



![image](https://github.com/user-attachments/assets/f25117ec-1982-4676-8e09-05d91508468f)

3) As quads are assigned, create a new folder with the quad number as a label within the relevant country folder.

![image](https://github.com/user-attachments/assets/eef90db7-2e3f-410b-bb7e-83e96db19c37)


4) Within each quad folder, there should be two folders: 'resources' and 'working'. Place each of the layers from sandy into the Resources folder.

![image](https://github.com/user-attachments/assets/a58dcf4e-530b-40db-a027-fecb5107f85a)


###  Setting up a project in Terrset

1) In Terrset, right click in the empty space of the 'projects' tab and select 'New Project'

![image](https://github.com/user-attachments/assets/c0051a12-4a76-4590-b35e-0e9fa6d28f0c)


2) Navigate to the working folder within the quad you're working on.

![image](https://github.com/user-attachments/assets/61ff0760-9e7c-45f4-b567-c54ceae8f581)

3) Change the name of the project from 'working' to the quad number

![image](https://github.com/user-attachments/assets/bfb0389e-334f-48d1-a741-55d774e9628f)

4) Add the resources and gis_files folders as resource folders. The completed setup should look like this.

![image](https://github.com/user-attachments/assets/f9506303-4997-4f79-b581-83a8d33a6620)

5) Start digitizing!


 
</details>


### Tutorial 2: What do these layers mean?

<details>
<summary>Layer Description</summary>

## Layer Description


Below is a description of each ogh the images used in digitizing mangroves.



| Layer Name                 | Description            | Preview      | 
|----------------------------|----------------------|-----------------|
| ![image](https://github.com/user-attachments/assets/3fd7206a-7b64-4605-8085-188ee5803222)     | Mask of Study area. <br> The study area for this project is 10 km on eihter side of the coast line, extending up to 60 km inland in low elevation areas.  |  ![image](https://github.com/user-attachments/assets/a22d9554-a2aa-48ee-a014-2e61d5f0e1ba) |
| ![image](https://github.com/user-attachments/assets/0f43b00b-0b62-47e7-9e7e-79833aa70565)     | Sentinel-1 [Synthetic Aperature Radar](https://www.earthdata.nasa.gov/learn/earth-observation-data-basics/sar) (SAR). <br> SAR imagery records the relative smoothness of the land surface. For example, the lowest values are found in smooth terrains such as open water and graded construction sites. The highest SAR values are found in complex terrains, such as mountainous terrains and dense urban areas. |    ![image](https://github.com/user-attachments/assets/e1559985-ed03-403f-a473-7adfa8f36492)  | 
| ![image](https://github.com/user-attachments/assets/af67fc90-e199-4fce-99e5-228bbaa108a6)    | Wetness image from the [tasseled cap transformation](https://pro.arcgis.com/en/pro-app/latest/help/analysis/raster-functions/tasseled-cap-function.htm). Note that highest wetness values are located in areas of open water and vegetation. Lowest wetness values are found in crop fields and built-up areas.    |  ![image](https://github.com/user-attachments/assets/097ebb71-1b8c-4d2f-9b7f-6c40bc97d894)  | 
|![image](https://github.com/user-attachments/assets/b095d101-0ae3-4334-9451-4512a104d75c) | False color composite using red, near infrared, and shortwave infrared bands. <br> Note that mangroves appear as red, other vegetation as orange, crop fields and built-up areas as cyan, and open water as deep blue.    | ![image](https://github.com/user-attachments/assets/769e7b8f-cd1b-441b-9c82-184605797dc2)    |
| ![image](https://github.com/user-attachments/assets/29318205-d965-4ef4-ad7f-e0b861445d3e)         | Landcover layer from previous years to update. <br> Using the provided ‘aqua’ palette, mangroves are deep green, aquaculture is orange, water is light blue, and other is yellow.  | ![image](https://github.com/user-attachments/assets/ced519ed-9a42-4d34-bd4a-b07c9148f74e) | 
| ![image](https://github.com/user-attachments/assets/fedb4cc3-0ded-4849-a45e-082b0aadbffd) | Archival landcover and image composites. For each previous year (2022, 2020, 2018, 2014, 1999) there is one composite and one classified landcover layer. | |


 </details>

### Tutorial 3: Digitize
<details>

<summary>DIGITIZE</summary>

## Tutorial Data

* Data for DIGITIZE tutorial can be downloaded from this repo (tutorial_data.zip)

## Setting Up a New Project

* Launch TerrSet by clicking on the desktop icon or searching the application in Start menu on machine. This will load the liberaGIS splash screen on your monitor.

* Once loaded, locate the TerrSet Explorer panel on the left side of the screen. Here you can revisit previous projects, create new projects, and delete projects. Users can also assign their working and resource folders in the Explorer panel. The working folder is the default location for files created within TerrSet, while the resource folders are designed to help users organize their input data. 

* Right click in the Explorer panel and click New Project (alternatively press “Insert”). Within the digitize folder, locate the ecuador subfolderfolder downloaded for this tutorial and press OK. You will now see the ecuador project in your Explorer panel.

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



## DIGITIZE Module

* As can be seen, this landcover map has some noticeable errors and revisions that need to be made. To streamline the process of editing raster maps and vector files, TerrSet provides users the DIGITIZE module.

* To access the DIGITIZE module, users can select the DIGITIZE icon in the toolbar (red and yellow crosshair) when a display window is open. Traditionally, the DIGITIZE module was used to help users create vector layers, often for the purpose of drawing training sites. For this tutorial, we will be focusing on the option to use vector features to update raster image(s). 

* Click the radio button to make this option visible and note the 4 options available (All pixels within digitized features, One class within digitized features, Use mask file, Overlay cover digitized features with raster image). This tutorial will explore each of these and examples of when to apply the different options.



![image](https://github.com/user-attachments/assets/2a75bd16-7ffc-4602-b2c1-87b0d45e7bc7)



## DIGITIZE - All pixels within digitized features

* The first option, and often most utilized for our work, is to digitize all pixels within a digitized feature – that is to say that all pixels that overlap with the features digitized by the user will be updated with the respective new value. This is most often used when new features need to be manually drawn into the map (e.g. adding a new ponds, removing errors, etc.) We will now use this option to add ponds to the map

* Start by zooming in on the region of the map that is shown below. Once located, use the blend layer option in composer on the landcover map to reveal the landsat image below it. As can be seen, a new pond is present in the imagery, but is not reflected in our landcover mapping – let’s update this.



![image](https://github.com/user-attachments/assets/cf6c8ed4-2533-432b-8697-e57c72a604a5)



* With the landcover raster layer highlighted in the composer, click on the DIGITIZE icon and select the option to use vector features to update raster layer(s).  

* At the top of the form is the option to name the file – let’s call this file “add_pond” as we will be using it to add the pond aquculture category to our map and overwrite whatever the class was previously underneath the features drawn by the user.

* Layer type and palette for the vector layer can be left as the defaults (polygon, Qual)

* The New class ID option is very important. This is the class value that will be newly assigned during the update process. As we are adding ponds to our map (class 3) we can change this value to 3.

* The raster layer(s) to update option is also important – this is the raster image in your composer that will have the updates applied to. In our case we are updating the landcover_2024 raster, so make sure that is the layer highlighted (NOTE – this often leads to errors so make sure you are updating the correct layers with the correct values in application of quad editing)

* Select the first option (All pixels within digitized features) and press OK. This will launch the digitize tool by adding the vector layer to your composer and changing your cursor to a crosshair. At this point you are in DIGITIZE mode.



![image](https://github.com/user-attachments/assets/e46153f7-378e-4821-b36b-07f1d9484d25)



* While in DIGITIZE mode, the cursor will function as  crosshair that allows users to draw polygons onto their window, which will in turn be the vector features within which updates are applied. To start drawing a polygon, click on the map to where the boundaries of the pond system can be seen and start building out a polygon with each vertices added. Right clicking will end the polygon by connecting to the first vertex. Holding Shift key will allow the user to continuously draw the polygon (much like a pencil).

* Using the options shown above, draw out the aquaculture ponds to be updated in the map. Once completed, the polygon feature should appear on screen. 



![image](https://github.com/user-attachments/assets/b2e2dae6-fc57-4553-a8b6-4e5575e8167d)



* At this point, we could update the raster layer using the Save Digitized Data option (Red arrow next to Red X in toolbar). However, for training purposes we will explore how to delete polygons if mistakes are made (this often happens)

* With the add_pond vector layer highlighted in composer, click on the polygon with your cursor. You will see it selected on screen with the ID value (3). To delete the polygon, click the Red X in the toolbar (delete feature). Alternatively, press the “Delete” key with the feature selected on screen. As can be seen, the polygon feature has been successfully deleted from the vector layer.

* Now let’s get back to our task of adding ponds. To continue editing the raster as before, highlight the layer in composer and then press the DIGITIZE logo and select “continue to digitize features to update layer with.” Alternatively, press the “d” key with the layer selected in composer to quickly start digitizing again (this is another useful hot key that will make this process faster for the user).

* Draw in the new pond system as before, but this time press the red arrow icon in the toolbar (Save Digitized Data). When prompted to update the layer, press OK. The landcover map will now be updated with the new ponds and visible on screen.



![image](https://github.com/user-attachments/assets/9ec7c6f2-c0c1-4823-babb-af68d0bfb551)



## DIGITIZE - One class within digitized features

* Updating all features within drawn polygons is very useful, but sometimes you want to have more control over which features get updated, rather than an all-inclusive update. This presents itself contextually, but is still an essential option to know. Let’s explore a case where updating only a single class with the digitized features is the most efficient way to add changes

* Locate the region shown below – this is an area where the map is wrongfully categorizing mangrove (1) patches as water (4). When compared to the imagery, it is clear this is an artifact of map error and not the actual landscape.



![image](https://github.com/user-attachments/assets/d535bc52-3b4a-4ee4-a897-56d9311b2ae2)



* While we could update this using the option before (All pixels within digitized features), it would be awfully tedious and have a larger margin for user error. This is a perfect opportunity to use our second DIGITZE option (One class within digitized feature)

* Similar to before, highlight the landcover_2024 raster layer in composer and press the DIGITIZE icon (alternatively press “d”). Within the DIGITIZE form, change the name of the layer to be created to be “water_to_pond” and select update vector features to update raster layer(s) option. Change the new class ID to be 1 for mangroves and indicate the second option to be used (One class within digitized feature). The original ID value can be changed to 4 (water) as this is the class value we are updating (therefore, no other values besides 4 will be updated with the new value of 1 within our digitized features)



![image](https://github.com/user-attachments/assets/19c200b2-3a15-4360-9ca6-044be0ee0c0c)



* Press OK to launch the DIGITIZE mode. All the same controls as before apply, but the way in which the raster layer gets updated will be different. Unlike the first option, this option will allow us to generally circle the water classes to update to mangrove, without having to be sensitive of the other classes (as the only class to be updated within the features is 4).

* Draw a bounding polygon around the water in this area and close the feature.



![image](https://github.com/user-attachments/assets/fb235ac2-f946-4c1f-8e7d-1970fd97feb4)



* Press the Save Digitized Data icon and look at the landcover map. We have now successfully updated the water errors to mangrove, without sacrificing any of the other classes. 



![image](https://github.com/user-attachments/assets/cf02f8e8-e01d-4205-8520-281a66974ff7)



## DIGITIZE - Use mask file
 

* Often when digitizing, the need to restrict the updates to a certain region (as opposed to a certain class like the previous step) occurs. This can be for a variety of reasons (working on the edge of maps, updating from a pre-existing boolean image, etc.) and often leads to the need for a mask. This is the next option in the DIGITIZE module we will explore.

* Zoom in on the northwest corner of the map to the area shown below.



![image](https://github.com/user-attachments/assets/07c22dc6-3061-4300-81a7-55038658a4d1)



* As can be seen, there are errors in the map that appear as mangroves (1) and pond aquaculture (3) but are really other (5) in reality. Let’s fix this problem.

* One way we could fix this would be to digitize all these polygons by hand (option 1) but that would not only be time consuming, it would also leave room for error along the edge (we do not want to add areas into the map as categories when they should be background)

* Option 2 would allow us to update only certain classes within the digitized features, but we would need to run that twice (once for class 1 and once for class 3)

* This leads us to option 3, Updating using a mask file. This is an excellent example of when we would use this option as we are looking to update values along the edge of the map, but do not want to bleed outside the study area. 

* Go to the resource folder and add the mask to this composer window. Use the blend layer option in composer to compare the mask to the landcover_2024 map. Notice how this is a boolean raster image that has pixel values of 1 where we have map data and 0 where we do not (background). This is an appropriate map to use as a mask file.



![image](https://github.com/user-attachments/assets/69bf5d8b-cee8-4158-a834-ead114f020ba)



* Highlight the landcover_2024 raster in composer and launch the DIGITIZE form. Select the option to use vector features to update raster layer(s) and change the created layer name to be “add_other_masked.” Change the New class ID to be 5 (other) and select the third option (use mask file). Here you identify the mask layer by typing the name, choosing the file from the picklist option, or dragging and dropping the layer into the text box.



![image](https://github.com/user-attachments/assets/e4143873-de6c-402f-98ee-d8dc0dbd15bc)



* Press OK and digitize following the same controls as before. As we are updating all values within the mask we indicated, we should be able to easily circle the erroneous classes along the edge in one polygon, and update all values to the proper masked extent.



![image](https://github.com/user-attachments/assets/d92e2b26-0e74-4a37-84b4-55ebd5cafbd9)



* Once you have completed the polygon feature to update, press the Save Digitized Data (Red Arrow in toolbar) and update the raster image. The map will now properly display the category Other (5) along the edge of the map (without any bleeding outside the masked area)



![image](https://github.com/user-attachments/assets/cf71a744-cec9-4960-bc58-2f2c83f28a8f)



## DIGITIZE - Overlay cover digitized features with raster image



* The last option available to users is the Overlay cover digitized features with raster image. This is the option you will use the least for this research, but it is still important to know. This option allows users to cover the current image with ALL the classes of a different raster image that are within the digitized regions (i.e. to overlay cover one map on top of the other within the digitized regions). This can be helpful when you have a reference map that you are trying to cover on top of the edited map in specific areas.

* Zoom to the region shown in the display below. Notice how we are missing an entire chunk of the landcover map – this is a great case study for the fourth digitize option.

  

![image](https://github.com/user-attachments/assets/c7655320-a0b4-40ba-a485-08436c87a940)



* This tutorial includes a reference map that can be used to update the existing image you are editing. Add the file missing_landcover_2024 to your composer and toggle the transparency option in composer (right side of composer next to blue channel box) – notice how it provides the missing information we need (note, unless you are using the same palette it will appear in the default colors, but the values are correct)



![image](https://github.com/user-attachments/assets/1ee45969-d04d-4740-9787-1fb10357e9b0)



* Highlight the landcover_2024 raster in composer and launch the digitize form (note, make sure to highlight the correct raster as you should have multiple in your composer now) Select the option to use vector features to update raster layer(s). Name the file to be created add_cover and make sure the raster layer to be updated is landcover_2024. Select the fourth option (Overlay cover digitized features with raster image) and locate the missing_landcover_2024 image through the picklist, drag and drop, or typing in the short name



![image](https://github.com/user-attachments/assets/ddb56fd5-f525-466b-a0ca-b0ba7e94660a)



* Press OK and begin digitizing. We can cover the missing map on our existing landcover map for updates by circling it with a digitize feature.



![image](https://github.com/user-attachments/assets/b14b2342-a87a-4c9a-a97b-a22a8b55661a)



* Once finished digitizing, press Save Digitized Data (Red Arrow in toolbar) and OK to updated the raster image. The raster layer will now be updated with the missing information from the reference map.



![image](https://github.com/user-attachments/assets/5c36b4bd-22ea-4974-a584-de0aeea22741)



</details>

### Tutorial 4:Downloading and Importing Landsat Scenes

<details>



<summary>CP LANDSAT</summary>



## CP LANDSAT - Download Scene from Earth Explorer



* To download Landsat imagery for a quad, go to https://earthexplorer.usgs.gov/
	* EarthExplorer is the USGS-managed website that hosts earth observation data from a vairiety of sources, from Landsat to NOAA, and even some commercial sattelite data. The search options are powerful for choosing which image to select.

* Create a free EarthExplorer account by clicking the 'log in' button in the top right corner of the webpage, or log in if you have an existing account.
  
* Once you have logged in, select ‘path / row’ as your geocoding method

* Input the first three digits of your quad as the path number and the second three as the row number
  
* Constrain the dates between January 1st and December 31st for 2024.
  
* Click the 'data sets' button on the bottom of the screen to move to the data sets tab. 

  
![image](https://github.com/user-attachments/assets/3cccca91-1c71-45c2-9fb9-6fdc400d2080)


* In the data search list, under Landsat, select ‘Landsat Collection 2 Level 1’ and check the box for Landsat 8/9 OLI/TIRS C2 L1, then click the 'result' button to view the search results.
	* Collection 2 Level 1 contains preprocessed non-atmospherically corrected data that represents top-of-atmosphere (TOA) reflectance values. We're using this dataset becuase this is most similar to TOA reflectance data distributed from early Landsat sattelites.

![image](https://github.com/user-attachments/assets/2c6941db-92bb-44e1-b93b-32b097aa1db7)

* The results tab shows you images that match the search criteria entered in the search criteria and data sets tabs. 
* Examine the available images to find one with minimal clouds over the study area for your chosen quad.

![image](https://github.com/user-attachments/assets/8b393824-a714-4b9a-9194-c1f5bd846c1d)


* To download the image, select download, then product options, then download the product bundle.

![image](https://github.com/user-attachments/assets/21e8c309-cf34-463f-89a2-64725b50f8eb)

![image](https://github.com/user-attachments/assets/21a18e4f-1569-4933-b72e-1b9c3d115aa9)

## Extracting downloaded data

* The data will be downloaded as a .tar file
* Extract the file to a new folder within your quad folder named ‘landsat’
* Add the new ‘landsat’ folder as a resource folder to your terrset project.

![image](https://github.com/user-attachments/assets/24995d38-58eb-40c6-9edc-e87ff39058f7)

![image](https://github.com/user-attachments/assets/f12eb277-eacd-43a8-b6c0-2ed6b804fe00)


## Running CP Landsat

* Open the CP_Landsat tool.
* Select the file that ends in MTL.txt from the downloaded files.
	* This file records metadata for the scene, including band names, projection systems, data types, as well as attributes like image acquisition  time and sun angle. 
* As the mask, choose the study area mask from the resources folder.
* The tool will take a while (15-30 minutes) to run. 

  
![image](https://github.com/user-attachments/assets/0fb06571-ff8c-48f9-bec0-ddb51754ee9e)

* CP_Landsat imports the .tif files to .rst, then projects them to the desired coordinate system and performs the following functions:
* Images are pansharpened to 15 meter resolution.
	* The panchromatic band captures light across the visible spectrum (from 0.5 - 0.68 micrometers)at a 15m spatial resolution, compared to 30m pixel size for all other bands. The panchromatic band can then be used to increase the resolution of the red, green, and blue bands by combining the higher resolution imagery with the color information. See [here](https://up42.com/blog/how-pansharpening-improves-satellite-imagery) for more information of pansharpening.
 * The  [tasseled cap transformation](https://pro.arcgis.com/en/pro-app/latest/help/analysis/raster-functions/tasseled-cap-function.htm) is also run on the data.
	* Tasseled cap reduces the dimentionality of the data. By taking data from 6 bands and condensing it down to 3 images, it still retains important charactaristics about the land surface, and reduces processing time when further analyzing the imagery.
 	* The three output images are greeness, wetness, and brightness. Greenness represents healthy vegetation, while wetness measures surface water as well as moisture content in soil and vegetation. Brightness represents the overall albedo of ground objects. 


## CP Landsat Layer Outputs


| Layer Name              | Description                   | Preview      | 
|-------------------------|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| Q130052_20241221_band_1 | Coastal Aerosol               |   ![image](https://github.com/user-attachments/assets/92b00481-b4c9-4172-83be-64e25e28c547)  |
| Q130052_20241221_band_2 | Blue                          |   ![image](https://github.com/user-attachments/assets/30374887-55c2-4be3-bf84-11606051e8eb) | 
| Q130052_20241221_band_3 | Green                         |    ![image](https://github.com/user-attachments/assets/f25016a0-c785-409a-b9a4-a0c5df2ef03a)  | 
| Q130052_20241221_band_4 | Red                           |  ![image](https://github.com/user-attachments/assets/45dd1b7a-b806-4b67-95f9-6b08947e4958)  |
| Q130052_20241221_band_5 | Near-Infrared (NIR)           |    ![image](https://github.com/user-attachments/assets/8e9f88af-862e-4ff1-abce-3df5eaadadea) | 
| Q130052_20241221_band_6 | Shortwave Infrared 1 (SWIR1)  |   ![image](https://github.com/user-attachments/assets/51d6ca74-b2bd-463b-933e-ade512e17033) |
| Q130052_20241221_band_7 | Shortwave Infrared 2 (SWIR2)  |   ![image](https://github.com/user-attachments/assets/c0efee8b-46dc-4801-afb7-edad5c9fe275)   |
| Q130052_20241221_band_8 | Panchromatic                  |   ![image](https://github.com/user-attachments/assets/94f1eba9-6c30-4da9-9b00-b917baf59ef8)   |
| Q130052_20241221_composite456 | False Color Composite)  | ![image](https://github.com/user-attachments/assets/3b7aa040-1989-4d61-834c-56131e303af2) |
| Q130052_20241221_tass_bright  | Tasseled cap brightness | ![image](https://github.com/user-attachments/assets/8dcf6214-09a9-4006-a298-7fdf565fafb9)|
| Q130052_20241221_tass_green   | Tasseled cap greenness  |  ![image](https://github.com/user-attachments/assets/fccb44b1-bbcb-4845-abcb-7a2b4f0d990d) |
| Q130052_20241221_tass_wet     | Tasseled cap wetness    |  ![image](https://github.com/user-attachments/assets/822dd990-fee2-4bec-b310-196d10c6d023) |



</details>

### Tutorial 5: Image Classification
<details>

<summary>Mahalanobis Classification</summary>

## Tutorial data

* The data for this tutorial is provided as ___.zip
* Download ___.zip, extract the files, and set up a new project in Terrset using the working and resources folders included


* Here we see a large area within a quad is misclassified as not having any mangrove. Although we could manually digitize each patch of mangrove, with an environment so complex, it would take a long time and result in a less accurate classification than a model-based classification. 

![image](https://github.com/user-attachments/assets/537a458f-324d-4eca-9844-578fc73c8ccf)

## Creating Training sites

* Create a new vector file by opening hte digitize tool through the search bar or tool pane. For the name of the layer to be created, type 'trainmangrove'. Check the box for 'monitor training site areas', this will bring up a window showing the total number of pixels that have been selected for a particular class 
* Digitize some polygons within the areas of mangrove, making sure that all of the digitized polygons have the class listed as 1. These will be used as training sites for our automated classification.
	* It's important to ensure that you have captured a vaiery of areas within the class you wish to digitize, as classes such as mangrove have subtle variation in their reflectance values. A good rule of thumb is to add two or three new training sites each time you refine the classification, and keep each training site to no larger than 100 cells. 
 	* Make sure to save your digitized training sites before moving to the next step. 	

![image](https://github.com/user-attachments/assets/f1c1777c-d207-4e22-aa04-2f996c17fab8)

* Open ‘MAKESIG’
	* This tool will generate a signature file which stores the spectral properties of mangroves.  
* Define your training sites as ‘trainmangrove’
* Use the tasseled cap results under ‘bands to be processed’
	* The tasseled cap greenness, wetness, and brightness images will not take as long to process as using all of the bands. 
* Click ‘Enter signature file names…’ and input the signature name as mangrove and uncheck ‘create signature group file’

![image](https://github.com/user-attachments/assets/81e94e31-fc7f-4241-b1fc-c3ee8e30bd25)

* Open ‘Mahalclass’
	* This tool uses Mahalanobis distance to predict which pixels are most similar to those identified in the training samples. Unlike Euclidean (straight line) distance, Mahalanobis distance is a relative measure and it uses uses relationship between correlated variables to make calculate relative distance values. If you're interested in learning more about how Mahalanobis distance is calculated and applied, here are a few great resources: [a conceptual overview of the method](https://www.statisticshowto.com/mahalanobis-distance/) and [an applied classification example](https://www.machinelearningplus.com/statistics/mahalanobis-distance/).
* Choose ‘mangrove' as the signature file.
* Set the output prefix to ‘mahal’
* Check ‘Use Mask’ and select the study area mask for your quad

![image](https://github.com/user-attachments/assets/b835e85c-ead8-4cdf-86e1-56bd1533b4ff)


* After mahalclass has finished running, add the resulting mahalmangrove raster to your map window
* Toggle transparency and inspect the result
	* Mahalanobis is a soft classifier, meaning that it outputs typicality values representing how similar the classified pixel is to those identified in the training samples. Larger typicality values indicate that the identified pixel is more similar to the training samples.
* From this first run, we see that the the mangrove class is underrepresented, so more training samples will need to be added. Here, I go back to 'trainmangrove' polygon in the composer window and digitize 2-3 more training sites in areas where the model missed. If I saw overprediction in areas that are not mangrove, I would delete training sites in those areas. 

![image](https://github.com/user-attachments/assets/b6207035-2690-4905-ab36-6ed8b0711078)


* After iterating through these steps a few tmes, digitizing a few new training sites, then running makesig and mahalclass, then refining further, I have a classification I am happy with.
	* It is important to take an iterative approach to digitization rahter than classifying all of the mangrove at once, as this results in a much more accurate final product.
   
![image](https://github.com/user-attachments/assets/e5ca74d1-9c07-4eca-a2e5-54a5d1b08da7)

## Create Mangrove Mask

* To apply the classification to the image, we first have to change this from a soft classification to a hard classification, meaning that all of the pixels identified as mangrove are assigned a value of 1, and all pixels not mangrove are assigned a value of 0. To create this hard classification, use the reclass tool to reclassify all values less than 0.01 as zero, and any values greater than 0.01 as 1.
	* The Mahalanobis classification typically results in very small typicality values, you can choose any cutoff value you see fit, usually between 0.01 and 0.001.

![image](https://github.com/user-attachments/assets/4be7c38b-0c46-49be-a803-926186dd7a8b)

![image](https://github.com/user-attachments/assets/cbe425d8-64c7-423f-bc7d-b8490d3929c3)

## Add Mangrove to the Landcover Layer

* To add the classified mangrove to the landcover layer, first select the landcover layer, press ‘D’ to open the digitize pane. 
* Choose the 2024 landcover layer as the raster layer to update, and the new class ID as 1. Check ‘Use Mask file’ and select the reclassified mangrove classification from the previous step.

![image](https://github.com/user-attachments/assets/0bca2467-17d2-4428-adbf-285c7eac6996)

* Zoom to the area previously misclassified and draw a polygon around it 

![image](https://github.com/user-attachments/assets/2f72824a-7e2e-49e0-a8db-a09f2c4af97e)

* Save the vector layer and apply the edits to the landcover raster. 
* Now the landcover layer reflects the extent of mangroves accurately.

![image](https://github.com/user-attachments/assets/af6f81fb-e62b-4e44-ad5b-b91e51e50c5f)





</details>

</details>
