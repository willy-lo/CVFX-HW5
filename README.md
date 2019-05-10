# CVFX-HW5

1.Take multi-view images by yourselves

我們使用到了3種場景:

(1).校園草皮 
(2).台達二樓實驗室 
(3).資電外面樹木

2.原理:

移動視差 (motion parallax):

當我們往左方移動時，物體看起來會往右方移動。

較近的物體的位移 (displacement) 較明顯，較遠的物體的位移較不明顯。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut1.JPG)

單眼還根據許多其他較不明顯的線索判斷距離，列舉其中 2 項:

specific distance tendency

以下圖為例，以水平視角觀看物體時，認知的距離 (Per) 會比實際的距離 (Phy) 遠一些。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut2.JPG)

equidistance tendency

以下圖為例，看上方的物體時，認知的距離 (Per) 會比實際的距離 (Phy) 遠一些；看下方的物體時，認知的距離 (Per) 會比實際的距離 (Phy) 近一些。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut3.JPG)

這些判斷距離的線索都是觀察世界後學習得知的。

如下圖所示，透過數百萬張影像分析，人眼上方、水平、下方的物體出現的機率是不同的，由這樣的資料，可以解釋上述的判斷距離的線索。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut4.JPG)

3.Show image alignment results between different images

原圖:

reference:

4.Generate the multi-view 3D visual effects


5.Exploit creativity to add some image processing to enhance effect (Using post-production software is allowed)

