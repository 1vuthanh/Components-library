<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Component Library Diagram</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            padding: 20px;
        }
        
        .diagram {
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 900px;
        }
        
        .root {
            background-color: #f8c8e0;
            border-radius: 25px;
            padding: 10px 25px;
            text-align: center;
            font-weight: bold;
            margin-bottom: 20px;
            font-size: 18px;
        }
        
        .connection-line {
            width: 2px;
            height: 20px;
            background-color: #aaa;
            margin: 0 auto 10px;
        }
        
        .branches {
            display: flex;
            justify-content: space-around;
            width: 100%;
            gap: 15px;
        }
        
        .branch {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 100%;
            max-width: 200px;
            position: relative;
        }
        
        .branch:not(:last-child)::before {
            content: "";
            position: absolute;
            top: -20px;
            left: 50%;
            width: 100%;
            height: 2px;
            background-color: #aaa;
        }
        
        .main-box {
            background-color: #cfd8f7;
            border-radius: 20px;
            padding: 12px;
            text-align: center;
            width: 100%;
            box-sizing: border-box;
            font-weight: bold;
            margin-bottom: 20px;
        }
        
        .sub-box {
            background-color: #e6eafc;
            border-radius: 15px;
            padding: 10px;
            text-align: left;
            width: 100%;
            box-sizing: border-box;
            font-size: 14px;
        }
        
        .branch-line {
            width: 2px;
            height: 20px;
            background-color: #aaa;
            margin: 0 auto 10px;
        }
        
        ul {
            margin: 10px 0 0 0;
            padding-left: 20px;
        }
        
        li {
            margin-bottom: 5px;
        }
    </style>
</head>
<body>
    <div class="diagram">
        <!-- Root Node -->
        <div class="root">Component Library</div>
        
        <!-- Connection Line -->
        <div class="connection-line"></div>
        
        <!-- Main Branches -->
        <div class="branches">
            <!-- Atoms Branch -->
            <div class="branch">
                <div class="main-box">Atoms</div>
                <div class="branch-line"></div>
                <div class="sub-box">
                    Những component nhỏ, không thể tách rời:
                    <ul>
                        <li>Button (Primary, Secondary...)</li>
                    </ul>
                </div>
            </div>
            
            <!-- Molecules Branch -->
            <div class="branch">
                <div class="main-box">Molecules</div>
                <div class="branch-line"></div>
                <div class="sub-box">
                    Gồm nhiều atoms kết hợp với nhau:
                    <ul>
                        <li>Form Field (Input + Label + Error message...)</li>
                    </ul>
                </div>
            </div>
            
            <!-- Organisms Branch -->
            <div class="branch">
                <div class="main-box">Organisms...</div>
                <div class="branch-line"></div>
                <div class="sub-box">
                    Gồm nhiều molecules kết hợp:
                    <ul>
                        <li>Navbar (Logo + Menu + Search + Avatar)</li>
                    </ul>
                </div>
            </div>
            
            <!-- Templates & Pages Branch -->
            <div class="branch">
                <div class="main-box">Templates & Pages</div>
                <div class="branch-line"></div>
                <div class="sub-box">
                    Template: Cấu trúc trang (Dashboard layout, Sidebar layout...)
                    <br><br>
                    Page: Trang hoàn chỉnh...
                </div>
            </div>
        </div>
    </div>
</body>
</html>
