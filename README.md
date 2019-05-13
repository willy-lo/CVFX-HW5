# CVFX-HW5

1.Take multi-view images by yourselves

我們使用到了3種場景:

(1).校園草皮 

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/1%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/2%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/3%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/4%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/5%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/6%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/7%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/8%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/9%20resized.jpg)

(2).台達二樓實驗室 

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/10%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/11%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/12%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/25%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/26%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/27%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/40%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/41%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/42%20resized.jpg)



(3)資電外面樹木

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/43%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/44%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/46%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/47%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/49%20resized.jpg)
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/50%20resized.jpg)

2.原理或介紹:

motion parallax:

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

Stop motion:

定格動畫，又名逐幀動畫，是一種動畫技術，其原理即將每幀不同的圖像連續播放，從而產生動畫效果。最基本製作定格動畫的方法是利用相機作拍攝工具，為主要對象拍攝一連串的相片，每張相片之間為拍攝對象作小量移動，最後把整輯相片快速地連續播放便完成(每秒大約需要24張相片)。橡皮泥因為易於改動，是定格動畫常選用的材料，其成品被稱為黏土動畫。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut5.JPG)

要製作一條完整的定格動畫片，正如製作一般影片或動畫一樣，首先需要有一個故事、劇本甚或分鏡腳本。之後製作或搜集拍攝所需的模型或對象，如人物角式和場景等，並且作適當的燈光佈置。

完成前期工作後，再利用數位相機或攝影機，為這些預先製作好的對象拍攝大量連續的相片。視乎動畫使用的物料或對象，於相片與相片之間為模型或對象作小量移動，或轉換成不同的固定模型。拍攝完畢之後，把所有相片輸入在電腦中作排序。

定格動畫的拍攝對象可以千變萬化，可以是任何可以移動的物件，包括黏土、紙板或橡膠等製作成的模型或木偶、剪紙、日常用品以至真人等，另外亦可以用繪畫的方式製作。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut6.JPG)

定格動畫這藝術形式雖然已存在多年，但開始廣人們注目，是於2009年上映並被奧斯卡提名最佳動畫長片的定格動畫電影《第十四道門 Coraline》，這部片是美國奧勒岡的萊卡動畫工作室（Laika）的製作團隊打造而成。
 
第十四道門是改編英國知名作家尼爾蓋曼（Neil Gaiman）同名著作，以定格動畫打造出驚悚奇幻的黑暗童話故事；講述著卡洛琳女孩在只有十三間的新屋內發現了第十四扇門，於好奇心的驅使下，卡洛琳進入到第十四扇門內，並展開一段奇幻驚悚的旅程。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut7.JPG)

其第二部作品為《派拉諾曼-靈動小子 ParaNorman》於2012年結合3D打造出全新風格的恐怖喜劇，講述著能與死著溝通的諾曼，將設法拯救幾個世紀以來被詛咒的城鎮。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut8.JPG)

最新作品，《怪怪箱 Boxtrolls》是改編自艾朗司諾的幽默寓言小說《Here Be Monsters》，打造出非常可愛又害羞的生物，而且他們喜歡躲在可回收的紙板箱裡；他們收養了一個人類孤兒，而這個小男孩和一個愛冒險的地上世界女孩成為了好朋友，他們必需在怪物與人類之間建立一座橋樑—尤其是當人類政客為了選票而煽動民衆要把他們趕走…。

定格動畫最讓人欽佩的點，動畫師必須打造大至建築物，小至塵土的細節，並費其心思在每格畫面上細微的調整，例如：人物的移動、佈景的轉換、火焰水流煙霧等，讓每個細節以最逼真的方式活過來，若要呈現的是3D電影，那就必須要用3D攝影機拍攝兩次。

若要多個細微的東西一起移動，那真的是一項大工程，從影片中更可以看出萊卡打造的不是1:1的場景，而是等比例縮小的場景，讓已經如此迷你的世界，能夠栩栩如生的「動」起來，這工程肯定相當龐大；除了向傳統手工技法和定格動畫致敬，更引進3D技術，新舊技術的融合肯定讓影迷為之驚艷！

 Live photo:
 
 我們知道，iPhone 可以直接拍摄 Live Photo 来用做壁纸。可是那些自己拍摄、下载的视频怎麼轉换成 Live Photo 呢？以下推荐給你們这些App。
 
 intoLive:
 
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut9.JPG)
 
 打開 intoLive，選擇相片中的視頻、動畫、連拍快照或多张照片，「设置壁纸模式」—「→」—「不，重复」—「储存为 Live 照片」。
 
製作超過 5 秒的實況照片或使用高级功能需購買專業版。

imgLive:

這算是前一個App的豐富版。除了基本的轉Live Photo 功能，还有 Live Photo 轉成視頻、Gif 等操作。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut13.JPG)

App還有11首内置音樂，可供你添加到Live Photo，你還可以像制作視頻那样，調整視頻和音樂的音量大小。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut14.JPG)

而且它有一個我很喜欢的「情侣分屏模式Live照片」，也就是兩台手機同時播放的Live Photo可以组成一個視頻畫面。但这個功能需要升级到高级版本才能使用。

GIPHY:

世界上最大的動態 gif 和貼紙庫。你不僅可以將自己拍摄的視頻轉成Live Photo，還可以把裡面大量的Gif轉成Live Photo。搜索「KITTY」，馬上出現超多可爱的猫咪！

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut15.JPG)

選擇壁纸格式，就可以直接生成可爱的Live Photo了!

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut10.JPG)

Lumyer:

這個 App 可以给你拍摄的視頻添加特效。

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/live4.gif)

打開App，選擇Video，選擇喜欢的特效進行拍摄即可。


![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut11.JPG)

免费特效共有11個，其他特效需購買。


![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/cut12.JPG)

Lumyer還可直接將動畫保存成Live Photo格式，超方便。

3.Show image alignment results between different images

我們這組採用的樹來做模擬，分別對alignment的係數做不同的模擬，一個是係數為500的時候，另一個則是係數為5000的時候，可以看得出係數5000的效果比500好!之後貼上來的GIF我們則是用係數為5000的來創造出來!

原圖:

reference:

alignment=500:
 
![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/aligned50_500%20resized.jpg)
 
match=500:

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/matches50_500%20resized.jpg)

alignment=5000:

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/aligned50_5000%20resized.jpg)
 
match=5000:

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/matches50_5000%20resized.jpg)

4.Generate the multi-view 3D visual effects

motion parallax:

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_tree_org.gif)

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_tree_500.gif)

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_tree_5000.gif)

Stop motion:

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/lab_org.gif)

![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/lab_5000.gif)

 Live photo:
 
 ![image](https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_flag_org.gif)
 
 ![image]( https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_flag_500.gif)
 
 ![image]( https://github.com/willy-lo/CVFX-HW5/blob/master/cv_hw5/re_flag_5000.gif)

5.Exploit creativity to add some image processing to enhance effect (Using post-production software is allowed)

