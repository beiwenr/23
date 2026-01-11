# 23
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>保温上人屋面施工技术图</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Microsoft YaHei', 'Segoe UI', sans-serif;
        }
        body {
            background-color: #f8fafc;
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
        }
        header {
            text-align: center;
            margin-bottom: 30px;
            padding: 25px 20px;
            background-color: #7EC8E3; /* 调整饱和度的天蓝色 */
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(126, 200, 227, 0.15);
            color: white;
        }
        header h1 {
            color: white;
            margin-bottom: 12px;
            font-size: 1.8em;
        }
        .subtitle {
            color: rgba(255, 255, 255, 0.95);
            font-size: 1.1em;
            font-weight: normal;
        }
        .model-info {
            background-color: #f0f7fa;
            border-left: 4px solid #7EC8E3;
            padding: 12px 15px;
            margin-bottom: 20px;
            font-size: 0.9em;
            color: #2c6a8d;
            border-radius: 0 4px 4px 0;
        }
        .comparison-section {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 40px;
        }
        .comparison-item {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            overflow: hidden;
            display: flex;
            flex-direction: column;
        }
        .comparison-header {
            background: #5CB85C; /* 调整饱和度的绿色 */
            color: white;
            padding: 12px 20px;
            font-weight: bold;
            text-align: center;
        }
        .model-container, .plan-container {
            flex-grow: 1;
            min-height: 400px;
            position: relative;
        }
        #sketchfab-embed {
            width: 100%;
            height: 100%;
            border: none;
        }
        .plan-image {
            width: 100%;
            height: 100%;
            object-fit: contain;
            display: block;
            padding: 15px;
            background-color: #fff;
        }
        .content-section {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 30px;
        }
        .card {
            flex: 1;
            min-width: 300px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            overflow: hidden;
        }
        .card-header {
            background: #8E44AD; /* 调整饱和度的紫色 */
            color: white;
            padding: 15px 20px;
            font-weight: bold;
            font-size: 1.2em;
        }
        .card-content {
            padding: 20px;
        }
        .card-content ul {
            list-style-position: inside;
            margin-bottom: 15px;
        }
        .card-content li {
            margin-bottom: 10px;
            padding-left: 10px;
            border-left: 3px solid #E8DAEF;
            margin-left: 5px;
        }
        .step-list {
            counter-reset: step-counter;
        }
        .step-list li {
            counter-increment: step-counter;
            margin-bottom: 25px;
            padding-left: 110px;
            position: relative;
            list-style: none;
            min-height: 40px;
            border-left: 3px solid #E8DAEF;
            margin-left: 5px;
        }
        .step-list li::before {
            content: "步骤 " counter(step-counter);
            position: absolute;
            left: 0;
            top: 0;
            background: #8E44AD;
            color: white;
            font-weight: bold;
            padding: 8px 15px;
            border-radius: 4px;
            font-size: 0.9em;
            width: 90px;
            text-align: center;
            box-sizing: border-box;
            line-height: 1.4;
        }
        .step-list li strong {
            display: block;
            margin-bottom: 5px;
            font-size: 1.05em;
            color: #6C3483;
        }
        .step-detail {
            display: block;
            padding-top: 5px;
            line-height: 1.5;
        }
        .warning {
            background-color: #F4ECF7;
            border-left: 4px solid #8E44AD;
            padding: 15px;
            margin-top: 25px;
            border-radius: 0 4px 4px 0;
            color: #512E5F;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #E8DAEF;
            color: #6C3483;
            font-size: 0.9em;
        }
        footer a {
            color: #5CB85C;
            text-decoration: none;
        }
        footer a:hover {
            text-decoration: underline;
        }
        @media (max-width: 768px) {
            .comparison-section, .content-section {
                flex-direction: column;
            }
            .model-container, .plan-container {
                min-height: 300px;
            }
            .step-list li {
                padding-left: 100px;
            }
            .step-list li::before {
                width: 85px;
                padding: 6px 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>保温上人屋面施工技术详解</h1>
            <p class="subtitle">3D效果图、平面图与施工指导</p>
        </header>

        <div class="model-info">
            <p><strong>3D模型信息</strong> | 来源：Sketchfab | 作者：Bo-Zan-Li-Zi | 发布日期：2026年1月9日 | 面数：58.3k三角面</p>
        </div>

        <section class="comparison-section">
            <div class="comparison-item">
                <div class="comparison-header">3D效果图</div>
                <div class="model-container">
                    <!-- 嵌入来自Sketchfab的3D模型 -->
                    <iframe id="sketchfab-embed"
                            title="保温上人屋面 3D模型"
                            allow="autoplay; fullscreen; xr-spatial-tracking"
                            xr-spatial-tracking
                            execution-while-out-of-viewport
                            execution-while-not-rendered
                            web-share
                            allowfullscreen
                            mozallowfullscreen="true"
                            webkitallowfullscreen="true"
                            src="https://sketchfab.com/models/9e7d2616f8cb4e50b847149f049a0063/embed?autospin=1&autostart=1&ui_controls=1&ui_infos=1&ui_stop=1&ui_watermark_link=0&ui_watermark=0">
                    </iframe>
                </div>
            </div>
            <div class="comparison-item">
                <div class="comparison-header">平面效果图</div>
                <div class="plan-container">
                    <!-- 更新为新的平面效果图 -->
                    <img src="https://image2url.com/r2/bucket3/images/1768103834238-53b60e00-21d9-447c-b623-daefd31c7982.png" 
                         alt="保温上人屋面平面图" 
                         class="plan-image">
                </div>
            </div>
        </section>

        <section class="content-section">
            <div class="card">
                <div class="card-header">施工注意事项</div>
                <div class="card-content">
                    <ul>
                        <li><strong>基层处理</strong>：施工前必须将结构基层清理干净，确保平整、牢固、无松动、无起砂。阴阳角应做成圆弧形。</li>
                        <li><strong>材料准备</strong>：保温材料、防水卷材等进场需有合格证并按规定复检。材料应分类堆放整齐，注意防火、防潮。</li>
                        <li><strong>坡度控制</strong>：严格按照设计图纸找坡，确保屋面排水通畅，无积水。平屋面排水坡度一般不小于2%。</li>
                        <li><strong>节点处理</strong>：屋面与女儿墙、出屋面管道、设备基础等交接处是防水的薄弱环节，需做附加防水层，确保密封严密。</li>
                        <li><strong>施工环境</strong>：防水层和保温层施工宜在晴天进行，基层应干燥。五级风及以上或雨雪天气不得施工。</li>
                        <li><strong>成品保护</strong>：每道工序完成后应及时验收，后续施工中应注意保护已完工的保温层、防水层，避免穿刺破坏。</li>
                    </ul>
                </div>
            </div>
            <div class="card">
                <div class="card-header">施工流程</div>
                <div class="card-content">
                    <ol class="step-list">
                        <li>
                            <strong>基层清理与处理</strong>
                            <span class="step-detail">清除屋面板上的杂物、灰尘，修补孔洞和裂缝，保证基层坚实、平整、干净。</span>
                        </li>
                        <li>
                            <strong>找坡层施工</strong>
                            <span class="step-detail">按设计坡度要求，用水泥陶粒混凝土或轻质砂浆铺设找坡层，形成屋面排水坡度。</span>
                        </li>
                        <li>
                            <strong>保温层铺设</strong>
                            <span class="step-detail">将预制保温板（如XPS挤塑板、EPS聚苯板）紧密铺贴，板缝错开，并用专用胶粘剂固定。</span>
                        </li>
                        <li>
                            <strong>找平层施工</strong>
                            <span class="step-detail">在保温层上做水泥砂浆找平层，表面压光，为防水层施工提供平整基层。</span>
                        </li>
                        <li>
                            <strong>防水层施工</strong>
                            <span class="step-detail">先涂刷基层处理剂，然后铺贴防水卷材（SBS、APP等）。卷材搭接宽度应符合规范，热熔封边。</span>
                        </li>
                        <li>
                            <strong>保护层施工</strong>
                            <span class="step-detail">防水层验收合格后，铺设隔离层，再浇筑细石混凝土保护层（配筋）或铺设面砖等上人面层。</span>
                        </li>
                        <li>
                            <strong>细部构造处理</strong>
                            <span class="step-detail">安装雨水口、排气孔，处理泛水、收头等细部节点，确保全屋面防水密闭。</span>
                        </li>
                        <li>
                            <strong>养护与验收</strong>
                            <span class="step-detail">保护层及时洒水养护。所有工序完成后，进行蓄水或淋水试验，验收合格后方可交付。</span>
                        </li>
                    </ol>
                </div>
            </div>
        </section>

        <div class="warning">
            <p><strong>重要提示：</strong> 本页提供的施工信息为基于常见屋面构造的<strong>通用性指导</strong>。实际施工必须严格遵循具体项目的<strong>设计图纸、施工规范及当地标准</strong>，并由专业技术人员负责。</p>
        </div>

        <footer>
            <p>© 2026 保温上人屋面施工技术参考 | 3D模型来源：<a href="https://sketchfab.com/Bo-Zan-Li-Zi" target="_blank">Sketchfab - Bo-Zan-Li-Zi</a></p>
            <p><em>注：平面效果图已更新为最新版本。</em></p>
        </footer>
    </div>
</body>
</html>
