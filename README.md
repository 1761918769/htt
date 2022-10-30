​<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <meta name="author" content="http://www.wuiso.com/"/>
    <title>抖音底部样式html代码</title></head><body>
<!--底部代码--><style>
footer {
    position: fixed;
    left: 0;
    bottom: 0;
    /*height: 2.59rem;*/
    width: 100%;
    background-color: #000;
    background-color: rgba(0, 0, 0, 0.84);
    border-top: 1px solid #e0e0e0;
    z-index: 999;
}footer>ul>li {
    float: left;
    width: 19%;
    text-align: center;
    font-size: 1rem;
    line-height: 39px;
}li {
    list-style: none;
}a {
        color: #fff;
    -webkit-backface-visibility: hidden;
    text-decoration: none;
}.router-link-exact-active {
    color: #fff;
    border-bottom: 1px solid #fff;
}.main2 {
    position: relative;
    color: #362732;
    background: #fff;
    border-radius: 8px;
    border-left: 2px solid rgba(23,255,232,.7);
    border-right: 2px solid rgba(254,44,85,.7);
}.g_wrap2 {
    text-shadow: -2px 0 rgba(0,255,255,.5), 2px 0 rgba(255,0,0,.5);
}.dropdown-ment {
    top: auto;
    bottom: 100%;
    margin-bottom: 2px;
    position: absolute;
    left: -3px;
    z-index: 1000;
    float: left;
    padding: 5px 0;
    margin: 2px 0 0;
    font-size: 16px;
    text-align: left;
    list-style: none;
    background-color: #000;
    background-color: rgba(0,0,0,.8);
    background-clip: padding-box;
    border: 1px solid #ccc;
    border: 1px solid rgba(0,0,0,.15);
    border-radius: 4px;
    box-shadow: 0 6px 12px rgba(0,0,0,.5);
}
#xylo{width: 60px;
    padding: 2px 6px;}</style>
<footer>
<ul style="border-top: 1px solid rgba(255, 255, 255, 0.2);margin: 0;padding: 0;">
<li><a href="#" class="router-link-exact-active nav-active">首页</a></li> 
<li><a href="#" class="">视频</a></li> <li class="main2">
<div class="g_wrap2" id="butt"><span style="padding-right: 5px;">≡</span>抖音</div> 
<ul class="dropdown-ment" id="xylo" style="display:none;"><li><a href="#">快手</a></li> 
<li><a href="#">美拍</a></li></ul></li> <li><a href="#" class="">网红</a></li> 
<li><a href="#" class="">音乐</a></li></ul> 
<div style="position: fixed; top: 0px; right: 0px; bottom: 0px; left: 0px; display: none;"></div>
</footer>
<script type="text/javascript">
        window.onload = function () {
            var obt = document.getElementById("butt");
            var odiv = document.getElementById("xylo");
            function getStyle(obj, attr) {  //  谁的      那个属性
                if (obj.currentStyle)  // ie 等
                {
                    return obj.currentStyle[attr];
                }
                else {
                    return window.getComputedStyle(obj, null)[attr];  // w3c 浏览器
                }
            }
            //console.log(getStyle(odiv, 'display'));
            obt.onclick = function () {
                //获取的样式需要写在点击事件里面，写在外面只能获取一次，不能动态获取，
                if (getStyle(odiv, 'display') == "none") {
                    odiv.style.display = "block";
                }
                else {
                    odiv.style.display = "none";
                }
            }
        }
    </script>
</body>
</html>


