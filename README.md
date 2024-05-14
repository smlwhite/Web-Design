# 大家好~主要介紹過去曾經架設的簡單網頁 

```html
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
    <div class="d-flex justify-content-center">
        <title></title>
    </div>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
```
## 在每一頁的基本架構~**網頁基底**
透過在**Header**導入bootstrapcdn、Jquery的方式來來設計每一頁面上方的幻燈片，在**Body**的位置製作**header、footer**和**幻燈片**。
### Header分頁
```html
<nav class="nav navbar-inverse">
        <div class="container-fluid">
            <div class="navbar-header">
                <a class="navbar-brand" href="index.html" >HOME</a>
            </div>
            <div class="navbar-header">
                <a class="navbar-brand" href="登山.html">登山</a>
            </div>            
            <div class="navbar-header">
                <a class="navbar-brand" href="露營.html">露營</a>
            </div>            
            <div class="navbar-header">
                <a class="navbar-brand" href="野炊.html">野炊</a>
            </div>
            <div class="navbar-header">
                <a class="navbar-brand" href="相關影片.html">相關影片</a>
            </div>            
        </div>
    </nav> 
```
這邊主要透過超連結的方式，將每個分頁串接起來，並設計在Head的位置，可以透過點擊文字切換頁面。
### 幻燈片
```html
<div class="container">
               <h2></h2>
        <div id="myCarousel" class="carousel slide" data-ride="carousel">
            <!-- 點點 -->
            <ol class="carousel-indicators">
                <li data-target="#myCarousel" data-slide-to="1" class="active"></li>
                <li data-target="#myCarousel" data-slide-to="2"></li>
                <li data-target="#myCarousel" data-slide-to="3"></li>
                <li data-target="#myCarousel" data-slide-to="4"></li>
                <li data-target="#myCarousel" data-slide-to="5"></li>
                <li data-target="#myCarousel" data-slide-to="6"></li>

            </ol>
            <script src="https://code.jquery.com/jquery.js"></script>
            <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/js/bootstrap.min.js"></script>
            
               <div class="jumbotron text-center">
                <h1>Natural Felling</h1>
                <p>Relax your body and walk into nature</p>
            </div>
            <div class="carousel-inner">
                <div class="item active">
                    <img src="幻燈片/1.jpg" style="width:100%">
                </div>
                <div class="item">
                    <img src="幻燈片/2.jpg" style="width:100%">
                </div>
                <div class="item">
                    <img src="幻燈片/3.jpg" style="width:100%">
                </div>
                <div class="item">
                    <img src="幻燈片/4.jpg" style="width:100%">
                </div>
                <div class="item">
                    <img src="幻燈片/5.jpg" style="width:100%">
                </div>
                <div class="item">
                    <img src="幻燈片/6.jpg" style="width:100%">
                </div>
            </div>
            <a href="#myCarousel" class="left carousel-control" data-slide="prev">
                <span class="glyphicon glyphicon-chevron-left"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a href="#myCarousel" class="right carousel-control" data-slide="next">
                <span class="glyphicon glyphicon-chevron-right"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>
```
這個部分主要在設計幻燈片有哪些圖片、幻燈片的順序以及圖片的大小等，並將這些設定為置中。另外可以看到在最下面**href=mycarousel**的位置，主要在設定說幻燈片切換下一張還是上一張。
### Footer設計
```html
<footer id="sticky-footer" class="py-4 bg-dark text-white-50">
    <div class="container text-center">
      <small>Design By Myself</small>
    </div>
  </footer>
```
最後的話就是設計一個簡單的頁尾來完成基本的模板~~
## Table應用
設定完相關的模板後開始設計其他分頁的內容，以簡單的方式呈現文字以及超連結來達到想要的位置，由於每一頁都是文字的基本介紹居多，所以用**爬山.html**這個分頁為範例向各位介紹如何排版的。
```html
        <div class="row">
            <div class="col-sm-3">
                <div class="d-flex justify-content-center">
                    <h3><a href="#a1">裝備</a></h3>
                </div>
            </div>
            <div class="col-sm-3">
                <div class="d-flex justify-content-center">
                    <h3><a href="#b">糧食</a></h3>
                </div>
            </div>
            <div class="col-sm-3">
                <div class="d-flex justify-content-center">
                    <h3><a href="#c">安全</a></h3>
                </div>
                </div>
            <div class="col-sm-3">
                <div class="d-flex justify-content-center">
                    <h3><a href="#d">高山症預防與處理</a></h3>
                </div>
            </div>
        </div>
```
首先，將大標題放置在幻燈片下方，並將標題設計為超連結，當點擊的時候可以直接跳到想要查看的位置。
```html
 <div class="container">
<table class="table table-dark">
  <thead>
    <tr>
      <th scope="col">食</th>
      <th scope="col">爐子(汽化爐、瓦斯爐)、燃料(配合所使用之爐具)、 炊具(組合式)、食具（碗筷）、水袋、糧食、行動糧、飲水（水壺）等</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">衣</th>
      <td>三層式穿法：內層排汗；以P.P排汗材質為佳。中層保暖；以羊毛、羽毛、派兒刷毛為主。外層防風雨；以兩截式防水透氣雨衣較好，如；GORE-TEX布料)。帽子(頭部毛細孔多散熱快，且腦部充滿微血管，一但失溫不易補回，很容易頭痛感冒)。登山衣褲以鮮豔為宜（如登山社團的制服都很鮮豔)。手套、口罩、頭巾等。VBL穿法(蒸氣阻隔保溫法)。原則：快乾、保暖、防水透氣、舒適、耐磨、鮮豔。</td>
    </tr>
    <tr>
      <th scope="row">住</th>
      <td>帳篷(內帳透氣不防水、因而內、外帳必需隔開)、睡袋（羽毛、中空纖維）、睡墊（防止體熱被大地吸走，重要性不亞於睡袋。鋁箔向下防潮，泡棉向上與身體接觸保暖）。露宿袋、睡袋內套、拖鞋、備用衣物（夜晚可穿上保暖亦可當枕頭）。</td>

    </tr>
    <tr>
      <th scope="row" >行</th>
      <td>背包（背包套）、防水袋、頭燈(LED省電)、登山仗、登山鞋(視地型、天數而樣式不一樣)、襪子、地圖、指北針、高度針(要常校正)、G.P.S、通訊設備（行動電話、無線電手機）、其它輔助器材等。</td>
    </tr>
  </tbody>
        </table></div><br><br><br>
    <div style="text-align:center;" id ="b"><h1>糧食</h1></div>
    <div class="container">
<table class="table table-dark">
  <thead>
    <tr>
      <th scope="col">一.</th>
      <th scope="col">登山飲食需攝取足夠的熱量及水份，食物以高醣、低脂為主，避免吃產氣食物(如豆類)及碳酸飲料。</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">二.</th>
      <td>登山飲食的準備，依個人每日營養需求量、活動天數估算所需的食物份量。準備原則：口味佳、體積小、重量輕、不易腐壞、調理快速簡單、營養高。</td>
    </tr>
    <tr>
      <th scope="row">三.</th>
      <td>登山前之進食不可過飽，行進中應適當補充水份及鹽分；飲水太多，可能加速體液中電解質之流失，並且增加體力消耗。</td>

    </tr>
    <tr>
      <th scope="row">四.</th>
      <td>預防脫水，脫水第一現象是疲勞，嚴重脫水會使呼吸急促、心跳加快或神智混淆，嚴重時會致命。</td>
    </tr>
        <tr>
      <th scope="row">五.</th>
      <td>登山請勿攜帶含酒精飲料，飲酒後雖可在短時內讓身體暖活，但因微血管擴張，也同時會消耗身体能量、增加失溫風險。</td>
    </tr>
        <tr>
      <th scope="row">六.</th>
      <td>缺氧需要較多醣類，因醣類消化吸收率高，容易轉換成活動能量。</td>
    </tr>
  </tbody>
```
這邊的話由於當初懶得排版，就直接用複製的方式呈現Table哈哈哈，並且設定Table的網底為黑色，字體為白色的樣式。
## 導入Youtube影片製作相關影片
那我們能透過**src**來導入外部影片，但這邊要注意的是如果該創作者更改為置或是將影片下架了會產生錯誤，但為了簡單呈現才用這種方式。
```html
<div class="container">
        <div class="row">
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/sydnuOMDdqs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/950PQEPCibA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>

        </div>
    </div>
<div style="text-align:center;" id ="b"><h1>露營</h1></div>
<div class="container">
        <div class="row">
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/39igGpTsiRI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/PHmmGtkMyrw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>

        </div>
    </div>
    <div style="text-align:center;" id ="c"><h1>野炊</h1></div>
<div class="container">
        <div class="row">
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/huVy22wTs_g" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="d-flex justify-content-center">
                    <h3><iframe width="560" height="315" src="https://www.youtube.com/embed/y-Vl7TxCo0s" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></h3>
                </div>
            </div>

        </div>
    </div>
```
我的話是用排版**2*3**的方式呈現影片，所以會是**col-sm-6**的方式來排列，如果要更改排列的方式就該這個部分就可以了，但還要稍微調整內容，製作到這邊基本上簡單的網頁設計就已經完成羅~但由於十分簡陋大家參考參考就好。

#結語
本來是為了期末作業才製作的網頁，但後來越做越覺得好玩所以開始找其他的元素開始加入，並且在最近開始重新經營Github，將自己學過的東西放置上來，雖然不是原創，而且都是跟網路上的不同創作者學來的，但還是希望稍微有幫助到大家一點點。最後成品的為這在這裡**https://smlwhite.github.io/Web-Design/** 點了就可以看羅。
