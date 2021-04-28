# chat_box_page_fb
iframe chat box page
```
<div class="boxfbchat" style="position: fixed; bottom: 0px; right: 0px; z-index: 500;">
  <div class="box_hotro">
    <span class="text">Bạn cần hỗ trợ </span>
  </div>
  <label for="navbar-toggle" class="close">Menu</label>
  <iframe src="https://www.facebook.com/plugins/page.php?href=link"
  width="250" height="250" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowtransparency="true">
  </iframe>
  
</div>
```

```css
.box_hotro {
    background: #c62860;
    color: #fff;
    height: 25px;
    position: absolute;
    left: 0;
    width: 230px;
    top: -45px;
    padding: 10px;
}
label.close {
    background: url(//img.zing.vn/products/vltkm/skin-2016/images/btn_close.gif) no-repeat;
}
label {
    color: #ccc;
    font-style: italic;
    display: block;
    width: 30px;
    height: 30px;
    background: #c62860;
    position: relative;
    text-indent: -9999px;
    cursor: pointer;
    position: absolute;
    right: 10px;
    top: -40px;
}
```

```javascript
if ($('.boxfbchat').length > 0) {
        $(".boxfbchat label").click(function() {
            if ($(this).hasClass("open")) {
                $(".boxfbchat").animate({
                    'bottom': 0
                }, 600);
                $(this).removeClass("open");
            } else {
                $(".boxfbchat").animate({
                    'bottom': -260
                }, 600);
                $(this).addClass("open");
            }
        })
    }
```
https://www.facebook.com/plugins/page.php?href=link_page&tabs=messages&width=250&height=250&small_header=true&adapt_container_width=false&hide_cover=true&show_facepile=false&appId=app_id_page
