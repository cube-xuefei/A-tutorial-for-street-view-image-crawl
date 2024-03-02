# A-tutorial-for-street-view-image-crawl

## 1. Intro
      To climb Street View Images, you need to use three tools:   
      a website that can download the city road network (eg: Open Street Map, Government website...),    
      a road network processing tool to obtain street view images' coordinates (arcgis, qgis...),   
      and a python interpreter to run the crawl program (pycharm, vscode,jupyter notebook...).     
   
      In this tutorial, I use Open Street Map, ArcGIS and pycharm. 

## 2. First Step: Download the city road network
      Open Street Map: https://www.openstreetmap.org/ 

## 3. Second Step: Obtain the coordinates of street view images   

   ### 3.1 Import the road network and clip it according to your study area boundaries    

       click "clip".    

<img width="1259" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/1580f50e-da9b-435a-a40d-d65c794014b6">   

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/7f704b33-cf68-42d7-af1a-187826faddef)   

   ### 3.2 Extract the centre line of roads (if your road dataset is the centre line road network, you could ignore this step.)   

       This step is mean to improve efficiency and avoid double sampling by merging roads too close.   

       3.2.1 create buffer for each roads.      

<img width="532" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/105d705e-f6c2-45b6-b658-70cb7a9c1c49">     

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/3fc5a422-e0eb-4c04-ab49-314e6bf6ef70)    

       3.2.2 Export buffer shapefile as tiff file.   

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/2d9e4277-856e-4eb2-8fd7-fc4c662a0fad)     

       click "zoom to layer"    

<img width="341" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/80e6f704-4cd8-43a4-b788-a545e7c6679a">    

       click "export map", notice you need to select buffer layer ONLY.    

<img width="490" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/a4f6852c-7491-42d1-9230-61624d1945aa">   

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/b72fe912-5b3b-4214-b462-6d80a285d3fe)    

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/e1f0ad81-c992-47f4-9af5-17b97dc00426)   


       import tiff file, click properties.    

<img width="341" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/aa84de9f-1a1c-4ee6-b723-1a4b80886a1a">   


![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/efa66351-01f4-455f-9036-bea14f770921)    

      add a new shapefile.

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/af23e44b-75a1-4dae-9b10-3902803f01de)     

     open Arcscan    

<img width="312" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/904692f8-3fa8-4753-b5a6-d0e65b17e557">   

     start edit this new shapefile.     

<img width="623" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/a1a309ec-e45e-4251-a1f5-acccd1ce8b1d">    

    click "options" (note: if you cannot use Arcscan, select customize----extensions-----enable Arcscan)     

<img width="580" alt="image" src="https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/5b4492a0-ceb8-4aa9-8573-3409a63ff620">        

![image](https://github.com/cube-xuefei/A-tutorial-for-street-view-image-crawl/assets/111174136/7071b67c-9040-4fa8-8095-de823d25c4b6)   






















       


   
 
