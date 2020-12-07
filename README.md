转自 https://www.52pojie.cn/thread-1236349-1-1.html 

介绍：
大家都知道，虽然现在天翼云有活动送会员，但每次都要用客户端下载，比较麻烦，所以就做了这个东西。HTML单页，如果有GitHub pages，就可以上传上去，直接就能用，配合IDM直接满速下载（如果嫌麻烦可以直接使用我自己搭建的网页：https://tmp.feilongproject.com/189cloud.html）.

源码为：
<html lang="zh-cn">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.0/dist/css/bootstrap.min.css">
        <title>天翼云盘快速下载</title>
        <style type="text/css">
            body {
                background-color: #0af;
            }
            .body {
                background-color: #0cf;
                width: 60%;
                margin: 15% auto;
                box-shadow: 0 0 32px 0 #808080;
                border-radius: 15px;
            }
            input {
                margin: 20px 20px;
                padding: 10px 10px;
                border: 1px solid #cdd;
                border-radius: 20px;
                width: 90%;
            }
            .tittle {
                text-align: center;
            }
            .download {
                text-align: center;
                margin: 20px 20px;
                padding: 10px 10px;
                border: 1px solid #cdd;
                border-radius: 20px;
            }
        </style>
    </head>
    <body>
        <div class="body">
            <h1 class="tittle">天翼云盘快速下载</h1>
            <hr />
            <form action="https://api.zzux.net/189/down.php" method="get" accept-charset="utf-8">
                <input type="url" name="url" placeholder="输入分享链接">
                <input type="text" name="password" placeholder="仅当有密码时填入密码">
                <button class="download" type="submit">现在下载</button>
            </form>
        </div>
    </body>
</html>

缺点及解决办法：
1：无法下载文件夹，只能下载文件。
解决办法：多个文件分别分享，分别下载（如果文件过多还是老老实实客户端下吧）；
2：可能有时下载不了（出现概率很低）。
解决办法：刷新一下网页再下载估计就可以了。



测试地址：https://greateday.github.io/189/
