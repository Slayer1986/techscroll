### 材料: 


Fonts：https://fonts.googleapis.com/

Bootstrap CDN：https://www.bootstrapcdn.com/

https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js

jquery-3.2.1.： https://code.jquery.com/

unpkg：https://unpkg.com/scrollreveal/dist/scrollreveal.min.js

img ：https://pixabay.com/  by [raniramli](https://pixabay.com/zh/users/raniramli-731298/)

##### 鸣谢 [ @Traversy Media](https://www.youtube.com/channel/UC29ju8bIPH5as8OGnQzwJyA)

> [TechScroll视频教学课](https://www.youtube.com/watch?v=ePgnR4gHIi4&t=109s)行翻墙边看边动手，也许你js对你来说是一脸懵B。慢慢来日子长了，即便你依旧不会读，但你会认识它们。推荐给喜欢网页设计的每一位和我一样的设计小白


but...你还可以做一个伸手党:
:bowtie: Live：https://slayer1986.github.io/techscroll/


```
<script
  src="https://code.jquery.com/jquery-3.2.1.js"
  integrity="sha256-DZAnKJ/6XZ9si04Hgrsxu/8s717jcIzLy3oi35EouyE="
  crossorigin="anonymous"></script>
```


```
<head>
    <meta charset="utf-8">
    <title>TechScroll</title>
    <link href="https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700%7CRoboto%7CJosefin+Sans:100,300,400,500" rel="stylesheet" type="text/css">
    <link rel="stylesheet" href="css/bootstrap.min.css">
    <link rel="stylesheet" href="css/style.css">
    <script src="https://unpkg.com/scrollreveal/dist/scrollreveal.min.js"></script>
  </head>
```

##### window.sr = ScrollReveal();

  
```
      window.sr = ScrollReveal();
      sr.reveal('.navbar', {
        duration: 2000,
        origin:'bottom'
      });
      sr.reveal('.showcase-left', {
        duration: 2000,
        origin:'top',
        distance:'300px'
      });
      sr.reveal('.showcase-right', {
        duration: 2000,
        origin:'right',
        distance:'300px'
      });
      sr.reveal('.showcase-btn', {
        duration: 2000,
        delay:2000,
        origin:'bottom'
      });
      sr.reveal('#testimonial div', {
        duration: 2000,
        origin:'bottom'
      });
      sr.reveal('.info-left', {
        duration: 2000,
        origin:'left',
        distance:'300px',
        viewFactor:0.2
      });
      sr.reveal('.info-right', {
        duration: 2000,
        origin:'right',
        distance:'300px',
        viewFactor:0.2
      });
<!-- END Window.sr-->
  <script>
    $(function() {
      // Smooth Scrolling
      $('a[href*="#"]:not([href="#"])').click(function() {
        if (location.pathname.replace(/^\//,'') == this.pathname.replace(/^\//,'') && location.hostname == this.hostname) {
          var target = $(this.hash);
          target = target.length ? target : $('[name=' + this.hash.slice(1) +']');
          if (target.length) {
            $('html, body').animate({
              scrollTop: target.offset().top
            }, 1000);
            return false;
          }
        }
      });
    });
    </script>
    ```
