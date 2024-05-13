我利用bootstape的模板<br>
https://getbootstrap.com/docs/4.4/components/carousel/ 為幻燈片學處習處<br> 
https://getbootstrap.com/docs/4.4/components/navbar/ 為導覽欄學處習處 <br>
https://getbootstrap.com/docs/4.4/layout/grid/ 為文字編輯模板以及封面編輯學習處
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
        #這邊是運用超連結與導覽欄的部分跟分頁連結起來
    <div class="container">
               <h2></h2>
        <div id="myCarousel" class="carousel slide" data-ride="carousel">
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
    #上面的話則是設定圖片大小後再設定DIV將圖片放進去，再與CSS連結達到幻燈片的效果
     <footer id="sticky-footer" class="py-4 bg-dark text-white-50">
     <div class="container text-center">
      <small>Design By Myself</small>
      </div>
     </footer>
    #這邊則是用footer語法做一個固定的頁尾
<div class="container">
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
    </div>
    #運用href達到索引效果，點下去後能索引到想要到的地方，並用"container"去做排版分區<br>
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
      <td>帳篷(內帳透氣不防水、因而內、外帳必需隔開)、睡袋（羽毛、中空纖維）、睡墊（防止體熱被大地吸走，重要性不亞於睡袋。鋁箔向下防潮，泡棉向上與身                  體接觸保暖）。露宿袋、睡袋內套、拖鞋、備用衣物（夜晚可穿上保暖亦可當枕頭）。</td>
  </tbody>
        </table>
        #這邊則是用了table-dark做一個黑色的文字排版<br>
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
 
 #這邊則是用HTML5的內建功能與影片連接，設定完邊框大小後再運用"container"去將影片至中
    
    
