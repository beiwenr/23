# 23
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>墙面工艺 - 3D效果与施工指南</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
            padding: 20px;
            max-width: 1400px;
            margin: 0 auto;
        }
        /* 版头色块 - 天蓝色 */
        header {
            text-align: center;
            margin-bottom: 30px;
            padding: 25px;
            border-radius: 12px;
            background: linear-gradient(135deg, #4FC3F7 0%, #29B6F6 100%);
            color: white;
            box-shadow: 0 6px 15px rgba(41, 182, 246, 0.2);
        }
        h1 {
            color: white;
            margin-bottom: 10px;
            font-size: 2.2em;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        .subtitle {
            color: rgba(255, 255, 255, 0.9);
            font-size: 1.1em;
        }
        /* 主要对比区域样式 */
        .comparison-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 40px;
        }
        /* 手机端双列布局调整 */
        @media (max-width: 768px) {
            .comparison-container {
                grid-template-columns: 1fr 1fr;
                gap: 15px;
            }
            .panel h2 {
                font-size: 1.2em;
                padding: 15px 15px;
            }
            .display-area {
                height: 250px;
            }
            .panel p {
                font-size: 0.85em;
                padding: 15px 15px 20px;
            }
        }
        @media (max-width: 480px) {
            .comparison-container {
                grid-template-columns: 1fr 1fr;
                gap: 12px;
            }
            .panel h2 {
                font-size: 1em;
                padding: 12px 12px;
            }
            .display-area {
                height: 200px;
            }
            .panel p {
                font-size: 0.8em;
                padding: 12px 12px 15px;
            }
            .panel h2 i {
                font-size: 0.9em;
                margin-right: 8px;
            }
        }
        .panel {
            background: white;
            border-radius: 12px;
            padding: 0;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            overflow: hidden;
        }
        .panel:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 20px rgba(0, 0, 0, 0.12);
        }
        /* 3D效果图与平面效果图标题区域 - 绿色背景 */
        .panel h2 {
            color: white;
            background: linear-gradient(135deg, #43A047 0%, #2E7D32 100%);
            padding: 18px 25px;
            margin: 0;
            font-size: 1.5em;
            border-radius: 12px 12px 0 0;
            display: flex;
            align-items: center;
        }
        .panel h2 i {
            margin-right: 12px;
            font-size: 1.2em;
        }
        /* 3D模型和平面图展示区 */
        .display-area {
            width: 100%;
            height: 380px;
            background: linear-gradient(145deg, #f5f5f5, #ececec);
            display: flex;
            align-items: center;
            justify-content: center;
            color: #888;
            font-size: 1.2em;
            border: none;
            margin: 0;
            overflow: hidden;
            padding: 10px;
        }
        .display-area iframe {
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 6px;
        }
        .display-area img {
            max-width: 100%;
            max-height: 100%;
            border-radius: 6px;
            object-fit: contain;
        }
        .panel p {
            color: #555;
            font-size: 0.95em;
            padding: 20px 25px 25px;
            margin: 0;
        }
        /* 施工信息区域样式 */
        .construction-info {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 30px;
        }
        /* 手机端施工信息区域双列布局调整 */
        @media (max-width: 768px) {
            .construction-info {
                grid-template-columns: 1fr 1fr;
                gap: 15px;
            }
            .info-section h2 {
                font-size: 1.2em;
                padding: 15px 15px;
            }
            .info-section-content {
                padding: 15px;
            }
            .warning-list li {
                padding: 10px 12px;
                margin-bottom: 10px;
                font-size: 0.85em;
            }
            .process-steps li {
                padding: 15px 15px 15px 60px;
                margin-bottom: 15px;
            }
            .step-title {
                font-size: 1em;
            }
            .step-desc {
                font-size: 0.85em;
            }
            .process-steps li:before {
                width: 30px;
                height: 30px;
                font-size: 1em;
            }
        }
        @media (max-width: 480px) {
            .construction-info {
                grid-template-columns: 1fr 1fr;
                gap: 12px;
            }
            .info-section h2 {
                font-size: 1em;
                padding: 12px 12px;
            }
            .info-section-content {
                padding: 12px;
            }
            .warning-list li {
                padding: 8px 10px;
                margin-bottom: 8px;
                font-size: 0.75em;
            }
            .process-steps li {
                padding: 12px 12px 12px 50px;
                margin-bottom: 12px;
            }
            .step-title {
                font-size: 0.9em;
            }
            .step-desc {
                font-size: 0.75em;
            }
            .process-steps li:before {
                width: 25px;
                height: 25px;
                font-size: 0.9em;
                left: 15px;
            }
            .info-section h2 i {
                font-size: 0.9em;
                margin-right: 8px;
            }
        }
        .info-section {
            background: white;
            border-radius: 12px;
            padding: 0;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.08);
            overflow: hidden;
        }
        /* 施工注意事项和施工流程标题区域 - 紫色背景 */
        .info-section h2 {
            color: white;
            background: linear-gradient(135deg, #7B1FA2 0%, #6A1B9A 100%);
            display: flex;
            align-items: center;
            margin: 0;
            padding: 20px 25px;
            border-radius: 12px 12px 0 0;
            font-size: 1.5em;
        }
        .info-section h2 i {
            margin-right: 12px;
            font-size: 1.2em;
        }
        .info-section-content {
            padding: 25px;
        }
        /* 注意事项列表 */
        .warning-list {
            list-style: none;
        }
        .warning-list li {
            padding: 14px 15px;
            margin-bottom: 12px;
            background-color: #f9f9f9;
            border-left: 4px solid #3498db;
            border-radius: 0 6px 6px 0;
            transition: all 0.2s ease;
        }
        .warning-list li:hover {
            background-color: #e3f2fd;
            border-left-color: #1a73e8;
        }
        .warning-list li strong {
            color: #2c3e50;
        }
        /* 施工流程步骤 */
        .process-steps {
            counter-reset: step-counter;
            list-style: none;
        }
        .process-steps li {
            counter-increment: step-counter;
            padding: 20px 20px 20px 70px;
            margin-bottom: 20px;
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            position: relative;
            border: 1px solid #eaeaea;
        }
        .process-steps li:before {
            content: counter(step-counter);
            position: absolute;
            left: 20px;
            top: 50%;
            transform: translateY(-50%);
            background: linear-gradient(135deg, #4a6fa5, #2c3e50);
            color: white;
            width: 36px;
            height: 36px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 1.1em;
        }
        .step-title {
            display: block;
            font-weight: bold;
            color: #2c3e50;
            margin-bottom: 8px;
            font-size: 1.1em;
        }
        .step-desc {
            color: #666;
            font-size: 0.95em;
        }
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #ddd;
            color: #7f8c8d;
            font-size: 0.9em;
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <header>
        <h1><i class="fas fa-paint-roller"></i> 墙面工艺详解</h1>
        <p class="subtitle">3D结构、平面效果与标准化施工指南</p>
    </header>

    <main>
        <section class="comparison-container">
            <!-- 左侧：3D效果图区域 -->
            <div class="panel">
                <h2><i class="fas fa-cube"></i> 3D工艺效果图</h2>
                <div class="display-area">
                    <!-- 请注意：你提供的Sketchfab模型无法在线加载，此处使用了原嵌入代码作为占位 -->
                    <!-- 请确保你的3D模型可以公开访问，或替换为其他可用的嵌入代码 -->
                    <iframe title="墙面工艺" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true"
                        allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport
                        execution-while-not-rendered web-share
                        src="https://sketchfab.com/models/e9633a81cf584a358aae98475066962c/embed?autospin=1&autostart=1&preload=1">
                    </iframe>
                </div>
                <p>此3D模型展示了墙面的分层结构与施工工艺。你可以使用鼠标旋转、缩放模型，从不同角度观察细节。</p>
            </div>

            <!-- 右侧：平面效果图区域 -->
            <div class="panel">
                <h2><i class="fas fa-image"></i> 平面施工图</h2>
                <div class="display-area">
                    <!-- 已更新为你提供的新图片链接 -->
                    <img src="https://image2url.com/r2/bucket3/images/1768048917525-b899ead1-ea34-46eb-9037-a1e046c342cf.png" alt="墙面平面施工图">
                </div>
                <p>平面图展示了墙面的尺寸、材料标注及关键施工节点。请结合3D模型对照查看。</p>
            </div>
        </section>

        <section class="construction-info">
            <!-- 左侧：施工注意事项 -->
            <div class="info-section">
                <h2><i class="fas fa-exclamation-triangle"></i> 施工注意事项</h2>
                <div class="info-section-content">
                    <ul class="warning-list">
                        <li><strong>基层处理：</strong>施工前必须确保墙面基层坚实、平整、无浮灰、无油污。空鼓、开裂处需彻底铲除并修补。</li>
                        <li><strong>环境要求：</strong>施工环境温度应保持在5℃-35℃，空气相对湿度低于85%。避免在雨天、大风天施工。</li>
                        <li><strong>材料调配：</strong>严格按照产品说明书的比例调配腻子、涂料等材料，并充分搅拌均匀。调配好的材料应在规定时间内用完。</li>
                        <li><strong>分层施工：</strong>腻子、底漆、面漆等每道工序必须待前一道完全干透后方可进行，严禁为赶工期强行施工。</li>
                        <li><strong>成品保护：</strong>施工中和施工后24小时内，应避免磕碰、淋水、暴晒，保持室内通风良好但避免强对流风直吹墙面。</li>
                        <li><strong>安全规范：</strong>高空作业必须搭建稳固脚手架，佩戴安全帽、安全带。施工现场注意防火，材料远离电源、火源。</li>
                    </ul>
                </div>
            </div>

            <!-- 右侧：施工流程 -->
            <div class="info-section">
                <h2><i class="fas fa-tasks"></i> 标准施工流程</h2>
                <div class="info-section-content">
                    <ol class="process-steps">
                        <li>
                            <span class="step-title">第一步：基层检查与处理</span>
                            <span class="step-desc">检查墙面空鼓、开裂、平整度与垂直度。铲除疏松层，用水泥砂浆或嵌缝石膏修补缺陷，彻底清洁表面。</span>
                        </li>
                        <li>
                            <span class="step-title">第二步：涂刷界面剂</span>
                            <span class="step-desc">均匀涂刷（或滚涂）墙体界面剂（墙固），增强基层附着力，封闭粉尘。确保涂刷到位，无遗漏。</span>
                        </li>
                        <li>
                            <span class="step-title">第三步：阴阳角处理与挂网</span>
                            <span class="step-desc">用靠尺和阴/阳角条处理所有阴阳角，确保顺直。在开槽处、新旧墙体接缝处等可能开裂的部位粘贴抗裂网格布。</span>
                        </li>
                        <li>
                            <span class="step-title">第四步：批刮腻子</span>
                            <span class="step-desc">通常批刮2-3遍。第一遍重在找平，后一遍重在收光。每遍厚度不宜超过2mm，干透后用砂纸打磨平整。</span>
                        </li>
                        <li>
                            <span class="step-title">第五步：打磨与清扫</span>
                            <span class="step-desc">使用灯泡照射辅助，用细砂纸（如240目以上）全面打磨至墙面平整光滑。打磨后务必用鸡毛掸子或湿布彻底清扫浮灰。</span>
                        </li>
                        <li>
                            <span class="step-title">第六步：涂刷底漆与面漆</span>
                            <span class="step-desc">先涂刷一遍抗碱底漆。干透后，涂刷两遍墙面面漆。涂刷应均匀，避免流挂、漏刷，滚涂纹理要细腻一致。</span>
                        </li>
                        <li>
                            <span class="step-title">第七步：验收与养护</span>
                            <span class="step-desc">检查墙面是否平整、无色差、无疙瘩、无刷痕。施工完毕后，建议养护7天以上，期间避免触碰和剧烈温湿度变化。</span>
                        </li>
                    </ol>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2026 墙面工艺施工指南 | 本页面内容仅供参考，具体施工请以实际设计方案和材料说明为准。</p>
        <p>最后更新日期：2026年1月10日</p>
    </footer>
</body>
</html>
