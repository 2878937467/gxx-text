10.21日测验
在本地创建一个文件夹叫test10.21 ,文件夹中应含有5个html文件,分别命名为1.html等.再创建一个readme.txt文件,将这几个问题贴如其中,最后将html中的js代码贴到答的下方.

1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:
<body>
    <div id="h1"></div>
    <script>
        var str=new String(123);
        var sstr=new String(456);
       document.getElementById('h1').innerText=str.concat(sstr);
      
    </script>
</body>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:
<body>
    <div id="h2"></div>
    <script>
        var str="87";
        var h2=document.getElementById('h2').innerText=str.padEnd(6,'0');
       
    </script>
</body>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:
<body>
    <h3 id="h3"></h3>
    <script>
        var str="79387.348";
        var h3=document.getElementById('h3').innerText=str.substr(0,8);
    </script>
</body>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:
<body>
    <h4 id="h4"></h4>
    <script>
         var href='img/head/icon/1.jpg';
        document.getElementById('h4').innerText=href.substring(0,14);
    </script>
</body>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:
