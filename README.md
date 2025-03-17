<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Component Library</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body { display: flex; justify-content: center; align-items: center; min-height: 100vh; background-color: #f8f9fa; }
        .chart { text-align: center; }
        .title { background: #ffb6c1; display: inline-block; padding: 10px 20px; border-radius: 10px; font-size: 20px; font-weight: bold; }
        .container { display: flex; justify-content: center; margin-top: 20px; gap: 20px; }
        .box { background: #d9e4fc; padding: 15px; border-radius: 10px; width: 180px; text-align: center; font-weight: bold; }
        .description { background: #eef2ff; padding: 10px; border-radius: 10px; margin-top: 10px; font-size: 14px; }
        .arrow { width: 2px; height: 20px; background: gray; margin: 10px auto; }
    </style>
</head>
<body>
    <div class="chart">
        <div class="title">Component Library</div>
        <div class="arrow"></div>
        <div class="container">
            <div>
                <div class="box">Atoms</div>
                <div class="arrow"></div>
                <div class="description">Những component nhỏ, không thể tách rời:<br>• Button (Primary, Secondary...)</div>
            </div>
            <div>
                <div class="box">Molecules</div>
                <div class="arrow"></div>
                <div class="description">Gồm nhiều atoms kết hợp với nhau:<br>• Form Field (Input + Label + Error message)</div>
            </div>
            <div>
                <div class="box">Organisms...</div>
                <div class="arrow"></div>
                <div class="description">Gồm nhiều molecules kết hợp:<br>• Navbar (Logo + Menu + Search + Avatar)</div>
            </div>
            <div>
                <div class="box">Templates & Pages</div>
                <div class="arrow"></div>
                <div class="description">Template: Cấu trúc trang (Dashboard layout, Sidebar layout...)<br>Page: Trang hoàn chỉnh</div>
            </div>
        </div>
    </div>
</body>
</html>
