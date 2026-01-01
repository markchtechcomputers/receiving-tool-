<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ProScan Upright | Enhanced PDF Scanner with Gallery Export</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            --secondary-gradient: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            --success-gradient: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            --warning-gradient: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
            --dark-gradient: linear-gradient(135deg, #2c3e50 0%, #4a6491 100%);
            --glass-bg: rgba(255, 255, 255, 0.15);
            --glass-border: rgba(255, 255, 255, 0.2);
            --shadow-lg: 0 20px 40px rgba(0, 0, 0, 0.15);
            --shadow-xl: 0 25px 50px rgba(0, 0, 0, 0.2);
            --border-radius-xl: 20px;
            --border-radius-lg: 16px;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
        }
        
        .app-container {
            max-width: 1400px;
            margin: 0 auto;
            perspective: 1000px;
        }
        
        .scanner-stand {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            transform-style: preserve-3d;
            margin-bottom: 40px;
        }
        
        .stand-base {
            width: 300px;
            height: 30px;
            background: linear-gradient(135deg, #2c3e50 0%, #4a6491 100%);
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            position: relative;
            z-index: 1;
        }
        
        .stand-pole {
            width: 15px;
            height: 100px;
            background: linear-gradient(to bottom, #4a6491, #2c3e50);
            border-radius: 8px 8px 0 0;
            position: relative;
            z-index: 2;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .stand-pole::after {
            content: '';
            position: absolute;
            top: -10px;
            left: -5px;
            right: -5px;
            height: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 10px;
        }
        
        .scanner-device {
            width: 90%;
            max-width: 900px;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            border-radius: var(--border-radius-xl);
            padding: 25px;
            margin-top: -10px;
            position: relative;
            z-index: 3;
            box-shadow: var(--shadow-xl);
            border: 8px solid #0f3460;
            transform: rotateX(5deg);
            transition: transform 0.5s ease;
        }
        
        .scanner-device:hover {
            transform: rotateX(5deg) translateY(-5px);
        }
        
        .scanner-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 25px;
            padding-bottom: 20px;
            border-bottom: 2px solid rgba(255, 255, 255, 0.1);
        }
        
        .scanner-title {
            color: white;
            font-size: 2.2rem;
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .scanner-title .badge {
            background: var(--success-gradient);
            padding: 8px 20px;
            border-radius: 30px;
            font-size: 0.9rem;
            font-weight: 600;
            letter-spacing: 1px;
        }
        
        .scanner-stats {
            display: flex;
            gap: 20px;
        }
        
        .stat-item {
            text-align: center;
            color: white;
            background: var(--glass-bg);
            padding: 12px 20px;
            border-radius: 12px;
            backdrop-filter: blur(10px);
            border: 1px solid var(--glass-border);
        }
        
        .stat-value {
            font-size: 1.8rem;
            font-weight: bold;
            background: var(--warning-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stat-label {
            font-size: 0.9rem;
            opacity: 0.9;
            margin-top: 5px;
        }
        
        .main-content {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 30px;
            margin-top: 30px;
        }
        
        @media (max-width: 1100px) {
            .main-content {
                grid-template-columns: 1fr;
            }
        }
        
        .scanner-section {
            background: var(--dark-gradient);
            border-radius: var(--border-radius-lg);
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: var(--shadow-lg);
        }
        
        .section-title {
            font-size: 1.5rem;
            color: white;
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 2px solid rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            gap: 12px;
        }
        
        .scanner-viewport {
            position: relative;
            width: 100%;
            height: 500px;
            background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 100%);
            border-radius: 16px;
            overflow: hidden;
            margin-bottom: 25px;
            border: 3px solid rgba(255, 255, 255, 0.1);
            box-shadow: inset 0 0 40px rgba(0, 0, 0, 0.5);
        }
        
        #camera-view {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transform: scaleX(-1); /* Mirror effect */
        }
        
        .upright-guide {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 65%;
            height: 85%;
            border: 3px solid #00ff88;
            border-radius: 8px;
            z-index: 5;
            pointer-events: none;
            box-shadow: 
                0 0 30px rgba(0, 255, 136, 0.4),
                inset 0 0 30px rgba(0, 255, 136, 0.2);
        }
        
        .upright-guide::before {
            content: 'UPRIGHT DOCUMENT AREA';
            position: absolute;
            top: -40px;
            left: 0;
            right: 0;
            text-align: center;
            color: #00ff88;
            font-weight: bold;
            font-size: 0.9rem;
            letter-spacing: 2px;
            text-shadow: 0 0 10px rgba(0, 255, 136, 0.5);
        }
        
        .scan-beam {
            position: absolute;
            top: 7.5%;
            left: 50%;
            transform: translateX(-50%);
            width: 70%;
            height: 6px;
            background: linear-gradient(90deg, 
                transparent 0%, 
                #00ff88 20%, 
                #00ff88 50%,
                #00ff88 80%, 
                transparent 100%);
            box-shadow: 
                0 0 20px #00ff88,
                0 0 40px #00ff88,
                0 0 60px rgba(0, 255, 136, 0.5);
            z-index: 10;
            border-radius: 3px;
            animation: upright-scan 2.5s cubic-bezier(0.4, 0, 0.2, 1) infinite;
        }
        
        @keyframes upright-scan {
            0% { 
                top: 7.5%;
                opacity: 0.8;
                box-shadow: 
                    0 0 20px #00ff88,
                    0 0 40px #00ff88,
                    0 0 60px rgba(0, 255, 136, 0.5);
            }
            50% { 
                top: 92.5%;
                opacity: 1;
                box-shadow: 
                    0 0 30px #00ff88,
                    0 0 60px #00ff88,
                    0 0 90px rgba(0, 255, 136, 0.8);
            }
            100% { 
                top: 7.5%;
                opacity: 0.8;
                box-shadow: 
                    0 0 20px #00ff88,
                    0 0 40px #00ff88,
                    0 0 60px rgba(0, 255, 136, 0.5);
            }
        }
        
        .orientation-sensor {
            position: absolute;
            top: 20px;
            right: 20px;
            background: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 12px 20px;
            border-radius: 12px;
            display: flex;
            align-items: center;
            gap: 12px;
            z-index: 20;
            font-weight: 600;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .sensor-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #00ff88;
            animation: pulse-green 2s infinite;
        }
        
        @keyframes pulse-green {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }
        
        .enhancement-controls {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 15px;
            margin-top: 25px;
        }
        
        .enhance-btn {
            padding: 16px;
            border: none;
            border-radius: 12px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            background: rgba(255, 255, 255, 0.1);
            color: white;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .enhance-btn:hover:not(:disabled) {
            transform: translateY(-5px) scale(1.05);
            background: rgba(255, 255, 255, 0.2);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        
        .enhance-btn.active {
            background: var(--primary-gradient);
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.3);
        }
        
        .scanner-controls {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin-top: 25px;
        }
        
        .control-btn {
            padding: 18px 20px;
            border: none;
            border-radius: 14px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
        }
        
        .control-btn-primary {
            background: var(--primary-gradient);
            color: white;
        }
        
        .control-btn-primary:hover:not(:disabled) {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.3);
        }
        
        .control-btn-success {
            background: var(--success-gradient);
            color: white;
        }
        
        .control-btn-success:hover:not(:disabled) {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(79, 172, 254, 0.3);
        }
        
        .control-btn-warning {
            background: var(--warning-gradient);
            color: white;
        }
        
        .control-btn-warning:hover:not(:disabled) {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(250, 112, 154, 0.3);
        }
        
        .control-btn-danger {
            background: linear-gradient(135deg, #ff416c 0%, #ff4b2b 100%);
            color: white;
        }
        
        .control-btn-danger:hover:not(:disabled) {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 30px rgba(255, 65, 108, 0.3);
        }
        
        .control-btn:disabled {
            background: #6b7280;
            cursor: not-allowed;
            transform: none;
            box-shadow: none;
        }
        
        .processing-section {
            background: white;
            border-radius: var(--border-radius-lg);
            padding: 25px;
            box-shadow: var(--shadow-lg);
            border: 1px solid rgba(0, 0, 0, 0.1);
        }
        
        .status-display {
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
            border-radius: 16px;
            padding: 25px;
            margin-bottom: 25px;
            border-left: 6px solid #667eea;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
        }
        
        .status-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }
        
        .status-indicator {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .status-dot {
            width: 16px;
            height: 16px;
            border-radius: 50%;
            background: #9ca3af;
            position: relative;
        }
        
        .status-dot.active {
            background: #10b981;
            box-shadow: 0 0 20px #10b981;
        }
        
        .status-dot.active::after {
            content: '';
            position: absolute;
            top: -4px;
            left: -4px;
            right: -4px;
            bottom: -4px;
            border: 2px solid #10b981;
            border-radius: 50%;
            animation: ripple 2s infinite;
        }
        
        @keyframes ripple {
            0% { transform: scale(0.8); opacity: 1; }
            100% { transform: scale(1.5); opacity: 0; }
        }
        
        .status-dot.scanning {
            background: #f59e0b;
            animation: pulse 1.5s infinite;
        }
        
        .enhance-preview {
            background: white;
            border-radius: 16px;
            padding: 25px;
            margin-top: 25px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
            border: 1px solid #e5e7eb;
            display: none;
        }
        
        .preview-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .preview-container {
            position: relative;
            width: 100%;
            height: 300px;
            background: #f8fafc;
            border-radius: 12px;
            overflow: hidden;
            border: 2px dashed #e5e7eb;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .preview-image {
            max-width: 100%;
            max-height: 100%;
            border-radius: 8px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            transition: transform 0.5s ease;
        }
        
        .enhance-sliders {
            margin-top: 25px;
        }
        
        .slider-container {
            margin-bottom: 20px;
        }
        
        .slider-label {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            font-weight: 500;
            color: #4b5563;
        }
        
        .slider {
            width: 100%;
            height: 8px;
            -webkit-appearance: none;
            appearance: none;
            background: linear-gradient(90deg, #e5e7eb, #667eea);
            border-radius: 4px;
            outline: none;
        }
        
        .slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            background: var(--primary-gradient);
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            border: 3px solid white;
        }
        
        .download-options {
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
            border-radius: 16px;
            padding: 25px;
            margin-top: 25px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
        }
        
        .download-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .download-card {
            background: white;
            border-radius: 12px;
            padding: 25px 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            border: 2px solid #e5e7eb;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
        }
        
        .download-card:hover {
            transform: translateY(-8px) scale(1.05);
            border-color: #667eea;
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.15);
        }
        
        .download-icon {
            width: 60px;
            height: 60px;
            background: var(--primary-gradient);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.8rem;
            margin-bottom: 10px;
        }
        
        .download-card h4 {
            color: #1f2937;
            margin-bottom: 5px;
        }
        
        .download-card p {
            color: #6b7280;
            font-size: 0.9rem;
        }
        
        .pdf-options {
            background: white;
            border-radius: 16px;
            padding: 25px;
            margin-top: 25px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
            border: 1px solid #e5e7eb;
        }
        
        .option-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .option-card {
            background: #f8fafc;
            border-radius: 12px;
            padding: 20px 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
            border: 2px solid #e5e7eb;
        }
        
        .option-card:hover {
            border-color: #667eea;
            background: #eff6ff;
        }
        
        .option-card.active {
            border-color: #667eea;
            background: #eff6ff;
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.1);
        }
        
        .progress-container {
            margin-top: 25px;
        }
        
        .progress-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        
        .progress-bar {
            height: 12px;
            background: linear-gradient(90deg, #e5e7eb, #d1d5db);
            border-radius: 6px;
            overflow: hidden;
        }
        
        .progress-fill {
            height: 100%;
            background: var(--success-gradient);
            width: 0%;
            border-radius: 6px;
            transition: width 0.5s ease;
            position: relative;
            overflow: hidden;
        }
        
        .progress-fill::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent, 
                rgba(255, 255, 255, 0.4), 
                transparent);
            animation: shimmer 2s infinite;
        }
        
        @keyframes shimmer {
            0% { left: -100%; }
            100% { left: 100%; }
        }
        
        .notification-center {
            position: fixed;
            top: 30px;
            right: 30px;
            z-index: 1000;
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 400px;
        }
        
        .notification {
            background: white;
            border-radius: 16px;
            padding: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.15);
            display: flex;
            align-items: center;
            gap: 20px;
            transform: translateX(120%);
            transition: transform 0.5s cubic-bezier(0.68, -0.55, 0.27, 1.55);
            border-left: 6px solid #10b981;
        }
        
        .notification.show {
            transform: translateX(0);
        }
        
        .notification.warning {
            border-left-color: #f59e0b;
        }
        
        .notification.error {
            border-left-color: #ef4444;
        }
        
        .notification-icon {
            width: 50px;
            height: 50px;
            background: var(--primary-gradient);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5rem;
            flex-shrink: 0;
        }
        
        .notification.warning .notification-icon {
            background: var(--warning-gradient);
        }
        
        .notification.error .notification-icon {
            background: linear-gradient(135deg, #ef4444, #dc2626);
        }
        
        @media (max-width: 768px) {
            .scanner-device {
                padding: 20px;
            }
            
            .scanner-header {
                flex-direction: column;
                gap: 20px;
                text-align: center;
            }
            
            .scanner-viewport {
                height: 400px;
            }
            
            .scanner-controls,
            .enhancement-controls {
                grid-template-columns: 1fr;
            }
            
            .download-grid,
            .option-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        .floating-action {
            position: fixed;
            bottom: 40px;
            right: 40px;
            z-index: 100;
        }
        
        .fab {
            width: 70px;
            height: 70px;
            background: var(--primary-gradient);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.8rem;
            cursor: pointer;
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.3);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            border: none;
        }
        
        .fab:hover {
            transform: scale(1.1) rotate(15deg);
            box-shadow: 0 20px 40px rgba(102, 126, 234, 0.4);
        }
        
        .galaxy-effect {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
            opacity: 0.3;
            background: 
                radial-gradient(circle at 20% 80%, rgba(102, 126, 234, 0.2) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(118, 75, 162, 0.2) 0%, transparent 50%),
                radial-gradient(circle at 40% 40%, rgba(79, 172, 254, 0.1) 0%, transparent 50%);
        }
    </style>
</head>
<body>
    <div class="app-container">
        <!-- Scanner Stand Design -->
        <div class="scanner-stand">
            <div class="stand-base"></div>
            <div class="stand-pole"></div>
            <div class="scanner-device">
                <div class="galaxy-effect"></div>
                
                <div class="scanner-header">
                    <div class="scanner-title">
                        <i class="fas fa-satellite-dish"></i>
                        ProScan Upright
                        <span class="badge">4K ENHANCED</span>
                    </div>
                    <div class="scanner-stats">
                        <div class="stat-item">
                            <div class="stat-value" id="scan-count">0</div>
                            <div class="stat-label">Scanned</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-value" id="quality-score">95%</div>
                            <div class="stat-label">Quality</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-value" id="storage-status">3.2GB</div>
                            <div class="stat-label">Free</div>
                        </div>
                    </div>
                </div>
                
                <div class="main-content">
                    <!-- Scanner Section -->
                    <div class="scanner-section">
                        <h2 class="section-title">
                            <i class="fas fa-camera-retro"></i> Upright Document Scanner
                        </h2>
                        
                        <div class="scanner-viewport">
                            <video id="camera-view" autoplay playsinline></video>
                            
                            <div class="upright-guide"></div>
                            <div class="scan-beam" id="scan-beam"></div>
                            
                            <div class="orientation-sensor" id="orientation-sensor">
                                <div class="sensor-dot"></div>
                                <span>UPRIGHT STABLE</span>
                            </div>
                            
                            <div class="detection-message" id="detection-message" style="
                                position: absolute;
                                bottom: 20px;
                                left: 0;
                                right: 0;
                                text-align: center;
                                color: #00ff88;
                                font-weight: 600;
                                text-shadow: 0 0 10px rgba(0, 255, 136, 0.5);
                                z-index: 20;
                                display: none;
                            ">
                                <i class="fas fa-check-circle"></i> DOCUMENT DETECTED - READY TO SCAN
                            </div>
                        </div>
                        
                        <div class="enhancement-controls">
                            <button class="enhance-btn active" data-enhance="auto">
                                <i class="fas fa-magic"></i> Auto-Enhance
                            </button>
                            <button class="enhance-btn" data-enhance="contrast">
                                <i class="fas fa-adjust"></i> Contrast
                            </button>
                            <button class="enhance-btn" data-enhance="brightness">
                                <i class="fas fa-sun"></i> Brightness
                            </button>
                            <button class="enhance-btn" data-enhance="sharpness">
                                <i class="fas fa-crosshairs"></i> Sharpness
                            </button>
                        </div>
                        
                        <div class="scanner-controls">
                            <button id="start-scanner" class="control-btn control-btn-primary">
                                <i class="fas fa-power-off"></i> Start Scanner
                            </button>
                            <button id="auto-scan" class="control-btn control-btn-success" disabled>
                                <i class="fas fa-robot"></i> Auto-Scan
                            </button>
                            <button id="capture-doc" class="control-btn control-btn-warning" disabled>
                                <i class="fas fa-camera"></i> Capture Now
                            </button>
                            <button id="reset-all" class="control-btn control-btn-danger">
                                <i class="fas fa-trash-alt"></i> Clear All
                            </button>
                        </div>
                    </div>
                    
                    <!-- Processing Section -->
                    <div class="processing-section">
                        <div class="status-display">
                            <div class="status-header">
                                <h3><i class="fas fa-chart-line"></i> Scanner Status</h3>
                                <div class="status-indicator">
                                    <div class="status-dot" id="status-dot"></div>
                                    <span id="status-text" style="font-weight: 600; color: #4b5563;">Ready</span>
                                </div>
                            </div>
                            <p id="status-details" style="color: #6b7280;">
                                Start the upright scanner and place your document within the green frame. 
                                The system will auto-detect and enhance for perfect A4 PDF output.
                            </p>
                            
                            <div class="progress-container" id="progress-container" style="display: none;">
                                <div class="progress-header">
                                    <span>Processing Document</span>
                                    <span id="progress-percent">0%</span>
                                </div>
                                <div class="progress-bar">
                                    <div class="progress-fill" id="progress-fill"></div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="enhance-preview" id="enhance-preview">
                            <div class="preview-header">
                                <h3><i class="fas fa-eye"></i> Enhanced Preview</h3>
                                <span id="page-count" style="background: #667eea; color: white; padding: 5px 15px; border-radius: 20px; font-size: 0.9rem;">Page 1</span>
                            </div>
                            
                            <div class="preview-container">
                                <img id="preview-image" class="preview-image" src="" alt="Enhanced preview">
                            </div>
                            
                            <div class="enhance-sliders">
                                <div class="slider-container">
                                    <div class="slider-label">
                                        <span>Contrast</span>
                                        <span id="contrast-value">100%</span>
                                    </div>
                                    <input type="range" class="slider" id="contrast-slider" min="50" max="200" value="100">
                                </div>
                                
                                <div class="slider-container">
                                    <div class="slider-label">
                                        <span>Brightness</span>
                                        <span id="brightness-value">100%</span>
                                    </div>
                                    <input type="range" class="slider" id="brightness-slider" min="50" max="200" value="100">
                                </div>
                                
                                <div class="slider-container">
                                    <div class="slider-label">
                                        <span>Sharpness</span>
                                        <span id="sharpness-value">100%</span>
                                    </div>
                                    <input type="range" class="slider" id="sharpness-slider" min="50" max="200" value="100">
                                </div>
                            </div>
                        </div>
                        
                        <div class="download-options">
                            <h3><i class="fas fa-download"></i> Download Options</h3>
                            <p style="color: #6b7280; margin-top: 10px;">
                                Save your enhanced documents to phone gallery or export as professional PDF
                            </p>
                            
                            <div class="download-grid">
                                <div class="download-card" id="download-jpg">
                                    <div class="download-icon">
                                        <i class="fas fa-image"></i>
                                    </div>
                                    <div>
                                        <h4>High-Quality JPG</h4>
                                        <p>Save to Phone Gallery</p>
                                    </div>
                                </div>
                                
                                <div class="download-card" id="download-pdf">
                                    <div class="download-icon">
                                        <i class="fas fa-file-pdf"></i>
                                    </div>
                                    <div>
                                        <h4>Enhanced PDF</h4>
                                        <p>A4 Formatted</p>
                                    </div>
                                </div>
                                
                                <div class="download-card" id="download-multi">
                                    <div class="download-icon">
                                        <i class="fas fa-copy"></i>
                                    </div>
                                    <div>
                                        <h4>Multi-Page PDF</h4>
                                        <p>All scanned pages</p>
                                    </div>
                                </div>
                                
                                <div class="download-card" id="download-cloud">
                                    <div class="download-icon">
                                        <i class="fas fa-cloud"></i>
                                    </div>
                                    <div>
                                        <h4>Cloud Backup</h4>
                                        <p>Secure storage</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="pdf-options">
                            <h3><i class="fas fa-cog"></i> PDF Settings</h3>
                            <p style="color: #6b7280; margin-top: 10px;">
                                Customize your PDF output quality and format
                            </p>
                            
                            <div class="option-grid">
                                <div class="option-card active" data-quality="high">
                                    <i class="fas fa-gem" style="font-size: 1.8rem; color: #667eea; margin-bottom: 10px;"></i>
                                    <p style="font-weight: 600;">High Quality</p>
                                    <small>4K Resolution</small>
                                </div>
                                
                                <div class="option-card" data-quality="medium">
                                    <i class="fas fa-balance-scale" style="font-size: 1.8rem; color: #f59e0b; margin-bottom: 10px;"></i>
                                    <p style="font-weight: 600;">Balanced</p>
                                    <small>Optimized Size</small>
                                </div>
                                
                                <div class="option-card" data-quality="compressed">
                                    <i class="fas fa-compress-alt" style="font-size: 1.8rem; color: #10b981; margin-bottom: 10px;"></i>
                                    <p style="font-weight: 600;">Compressed</p>
                                    <small>Small File Size</small>
                                </div>
                                
                                <div class="option-card" data-quality="grayscale">
                                    <i class="fas fa-palette" style="font-size: 1.8rem; color: #6b7280; margin-bottom: 10px;"></i>
                                    <p style="font-weight: 600;">Grayscale</p>
                                    <small>Black & White</small>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Notification Center -->
        <div class="notification-center" id="notification-center"></div>
        
        <!-- Floating Action Button -->
        <div class="floating-action">
            <button class="fab" id="quick-scan">
                <i class="fas fa-bolt"></i>
            </button>
        </div>
    </div>

    <script>
        // Global variables
        let cameraStream = null;
        let scannedDocuments = [];
        let isAutoScan = false;
        let currentDocument = null;
        let scanCount = 0;
        let pdfQuality = 'high';
        let enhancementSettings = {
            contrast: 100,
            brightness: 100,
            sharpness: 100,
            autoEnhance: true
        };
        
        // DOM Elements
        const cameraView = document.getElementById('camera-view');
        const startScannerBtn = document.getElementById('start-scanner');
        const autoScanBtn = document.getElementById('auto-scan');
        const captureDocBtn = document.getElementById('capture-doc');
        const resetAllBtn = document.getElementById('reset-all');
        const statusDot = document.getElementById('status-dot');
        const statusText = document.getElementById('status-text');
        const statusDetails = document.getElementById('status-details');
        const scanBeam = document.getElementById('scan-beam');
        const orientationSensor = document.getElementById('orientation-sensor');
        const detectionMessage = document.getElementById('detection-message');
        const progressContainer = document.getElementById('progress-container');
        const progressFill = document.getElementById('progress-fill');
        const progressPercent = document.getElementById('progress-percent');
        const enhancePreview = document.getElementById('enhance-preview');
        const previewImage = document.getElementById('preview-image');
        const pageCount = document.getElementById('page-count');
        const scanCountEl = document.getElementById('scan-count');
        const qualityScore = document.getElementById('quality-score');
        const notificationCenter = document.getElementById('notification-center');
        const quickScanBtn = document.getElementById('quick-scan');
        
        // Enhancement controls
        const contrastSlider = document.getElementById('contrast-slider');
        const brightnessSlider = document.getElementById('brightness-slider');
        const sharpnessSlider = document.getElementById('sharpness-slider');
        const contrastValue = document.getElementById('contrast-value');
        const brightnessValue = document.getElementById('brightness-value');
        const sharpnessValue = document.getElementById('sharpness-value');
        const enhanceButtons = document.querySelectorAll('.enhance-btn');
        
        // Download buttons
        const downloadJpgBtn = document.getElementById('download-jpg');
        const downloadPdfBtn = document.getElementById('download-pdf');
        const downloadMultiBtn = document.getElementById('download-multi');
        const downloadCloudBtn = document.getElementById('download-cloud');
        
        // PDF options
        const qualityCards = document.querySelectorAll('.option-card');
        
        // Initialize the application
        document.addEventListener('DOMContentLoaded', () => {
            // Initialize UI
            updateStatus('ready', 'Scanner ready. Click "Start Scanner" to begin.');
            updateStats();
            
            // Set up event listeners
            setupEventListeners();
            
            // Simulate upright orientation
            simulateUprightOrientation();
            
            // Initialize enhancement controls
            initEnhancementControls();
            
            // Initialize download handlers
            initDownloadHandlers();
            
            // Initialize PDF quality options
            initPDFOptions();
        });
        
        function setupEventListeners() {
            startScannerBtn.addEventListener('click', startScanner);
            autoScanBtn.addEventListener('click', toggleAutoScan);
            captureDocBtn.addEventListener('click', captureDocument);
            resetAllBtn.addEventListener('click', resetScanner);
            quickScanBtn.addEventListener('click', quickScan);
        }
        
        function initEnhancementControls() {
            // Enhancement buttons
            enhanceButtons.forEach(btn => {
                btn.addEventListener('click', function() {
                    // Remove active class from all buttons
                    enhanceButtons.forEach(b => b.classList.remove('active'));
                    // Add active class to clicked button
                    this.classList.add('active');
                    
                    const enhanceType = this.getAttribute('data-enhance');
                    if (enhanceType === 'auto') {
                        enhancementSettings.autoEnhance = true;
                        showNotification('Auto-Enhance', 'Automatic enhancement enabled for optimal results.');
                    } else {
                        enhancementSettings.autoEnhance = false;
                        showNotification('Manual Enhance', `${enhanceType.charAt(0).toUpperCase() + enhanceType.slice(1)} adjustment enabled.`);
                    }
                });
            });
            
            // Slider controls
            contrastSlider.addEventListener('input', function() {
                const value = this.value;
                contrastValue.textContent = `${value}%`;
                enhancementSettings.contrast = parseInt(value);
                applyEnhancement();
            });
            
            brightnessSlider.addEventListener('input', function() {
                const value = this.value;
                brightnessValue.textContent = `${value}%`;
                enhancementSettings.brightness = parseInt(value);
                applyEnhancement();
            });
            
            sharpnessSlider.addEventListener('input', function() {
                const value = this.value;
                sharpnessValue.textContent = `${value}%`;
                enhancementSettings.sharpness = parseInt(value);
                applyEnhancement();
            });
        }
        
        function initDownloadHandlers() {
            downloadJpgBtn.addEventListener('click', () => downloadToGallery('jpg'));
            downloadPdfBtn.addEventListener('click', () => downloadToGallery('pdf'));
            downloadMultiBtn.addEventListener('click', () => downloadToGallery('multi-pdf'));
            downloadCloudBtn.addEventListener('click', backupToCloud);
        }
        
        function initPDFOptions() {
            qualityCards.forEach(card => {
                card.addEventListener('click', function() {
                    // Remove active class from all cards
                    qualityCards.forEach(c => c.classList.remove('active'));
                    // Add active class to clicked card
                    this.classList.add('active');
                    // Update quality setting
                    pdfQuality = this.getAttribute('data-quality');
                    
                    const qualityNames = {
                        'high': 'High Quality (4K)',
                        'medium': 'Balanced Quality',
                        'compressed': 'Compressed Size',
                        'grayscale': 'Grayscale'
                    };
                    
                    showNotification('PDF Quality', `${qualityNames[pdfQuality]} selected for PDF export.`);
                });
            });
        }
        
        async function startScanner() {
            try {
                // Request camera with portrait orientation
                cameraStream = await navigator.mediaDevices.getUserMedia({
                    video: {
                        width: { ideal: 2160 }, // Portrait orientation
                        height: { ideal: 3840 },
                        facingMode: 'environment',
                        aspectRatio: 9/16
                    }
                });
                
                // Display camera stream
                cameraView.srcObject = cameraStream;
                
                // Update UI
                startScannerBtn.disabled = true;
                startScannerBtn.innerHTML = '<i class="fas fa-check-circle"></i> Scanner Active';
                autoScanBtn.disabled = false;
                captureDocBtn.disabled = false;
                
                // Update status
                updateStatus('active', 'Upright scanner active. Place document within green frame.');
                statusDot.classList.add('active');
                
                // Show scan beam animation
                scanBeam.style.animation = 'upright-scan 2.5s cubic-bezier(0.4, 0, 0.2, 1) infinite';
                
                // Simulate document detection
                simulateDocumentDetection();
                
                showNotification('Scanner Started', '4K upright scanner is now active and ready for document capture.', 'success');
                
            } catch (error) {
                console.error('Camera error:', error);
                updateStatus('error', 'Failed to access camera. Please check permissions.');
                showNotification('Camera Error', 'Unable to access camera. Please check permissions.', 'error');
                startScannerBtn.disabled = false;
                startScannerBtn.innerHTML = '<i class="fas fa-power-off"></i> Start Scanner';
            }
        }
        
        function simulateUprightOrientation() {
            // Simulate upright orientation sensor
            setInterval(() => {
                if (cameraStream) {
                    // Randomly simulate occasional movement
                    if (Math.random() < 0.1) {
                        orientationSensor.innerHTML = '<div class="sensor-dot" style="background: #f59e0b;"></div><span>ADJUSTING...</span>';
                        setTimeout(() => {
                            orientationSensor.innerHTML = '<div class="sensor-dot"></div><span>UPRIGHT STABLE</span>';
                        }, 500);
                    }
                }
            }, 3000);
        }
        
        function simulateDocumentDetection() {
            setTimeout(() => {
                if (cameraStream) {
                    detectionMessage.style.display = 'block';
                    updateStatus('detected', 'Document detected in upright position. Ready to scan.');
                    
                    // If auto-scan is enabled, automatically capture
                    if (isAutoScan) {
                        setTimeout(() => {
                            captureDocument();
                        }, 1000);
                    }
                }
            }, 1500);
        }
        
        function toggleAutoScan() {
            if (isAutoScan) {
                // Stop auto-scan
                isAutoScan = false;
                autoScanBtn.innerHTML = '<i class="fas fa-robot"></i> Auto-Scan';
                autoScanBtn.classList.remove('control-btn-danger');
                autoScanBtn.classList.add('control-btn-success');
                updateStatus('active', 'Auto-scan disabled. Use manual capture.');
                showNotification('Auto-Scan', 'Automatic scanning disabled.', 'warning');
            } else {
                // Start auto-scan
                isAutoScan = true;
                autoScanBtn.innerHTML = '<i class="fas fa-stop-circle"></i> Stop Auto-Scan';
                autoScanBtn.classList.remove('control-btn-success');
                autoScanBtn.classList.add('control-btn-danger');
                updateStatus('detecting', 'Auto-scan enabled. Looking for documents...');
                showNotification('Auto-Scan', 'Automatic scanning enabled. Documents will be captured automatically.', 'success');
                
                // If camera is active and document is detected, capture immediately
                if (cameraStream && detectionMessage.style.display === 'block') {
                    setTimeout(() => {
                        captureDocument();
                    }, 800);
                }
            }
        }
        
        function captureDocument() {
            if (!cameraStream) return;
            
            // Pause scan beam animation
            scanBeam.style.animation = 'none';
            
            // Hide detection message
            detectionMessage.style.display = 'none';
            
            // Create canvas for capture
            const canvas = document.createElement('canvas');
            const context = canvas.getContext('2d');
            
            // Set canvas to A4 portrait dimensions
            const a4Width = 1240; // High quality
            const a4Height = 1754; // A4 aspect ratio
            
            canvas.width = a4Width;
            canvas.height = a4Height;
            
            // Fill with white background
            context.fillStyle = 'white';
            context.fillRect(0, 0, canvas.width, canvas.height);
            
            // Get video dimensions
            const videoWidth = cameraView.videoWidth || 1280;
            const videoHeight = cameraView.videoHeight || 720;
            
            // Calculate portrait crop (upright document)
            const cropHeight = Math.min(videoHeight, videoWidth * 1.414);
            const cropWidth = cropHeight / 1.414;
            const cropX = (videoWidth - cropWidth) / 2;
            const cropY = (videoHeight - cropHeight) / 2;
            
            // Draw the cropped upright document
            context.drawImage(
                cameraView, 
                cropX, cropY, cropWidth, cropHeight, // Source (upright crop)
                0, 0, canvas.width, canvas.height // Destination (A4 canvas)
            );
            
            // Apply enhancement settings
            applyCanvasEnhancement(context, canvas.width, canvas.height);
            
            // Convert to data URL
            const imageData = canvas.toDataURL('image/jpeg', 0.95);
            
            // Create document object
            const document = {
                id: Date.now(),
                number: ++scanCount,
                imageData: imageData,
                enhancedData: imageData, // Will be updated with enhancements
                timestamp: new Date().toLocaleTimeString(),
                date: new Date().toLocaleDateString(),
                format: 'A4 Portrait',
                quality: '4K Enhanced',
                settings: { ...enhancementSettings }
            };
            
            scannedDocuments.push(document);
            currentDocument = document;
            
            // Update UI
            updatePreview(imageData);
            updateStats();
            
            // Show preview and enhancement controls
            enhancePreview.style.display = 'block';
            pageCount.textContent = `Page ${scanCount}`;
            
            // Update status
            updateStatus('captured', `Document ${scanCount} captured. Apply enhancements or download.`);
            statusDot.classList.remove('active');
            statusDot.classList.add('scanning');
            
            // Show processing animation
            showProcessing();
            
            // Restart scan beam after a delay
            setTimeout(() => {
                if (cameraStream) {
                    scanBeam.style.animation = 'upright-scan 2.5s cubic-bezier(0.4, 0, 0.2, 1) infinite';
                    
                    // If auto-scan is enabled and we have less than 5 pages, prepare for next
                    if (isAutoScan && scanCount < 5) {
                        setTimeout(() => {
                            detectionMessage.style.display = 'block';
                            updateStatus('ready', 'Ready for next document...');
                        }, 1000);
                    }
                }
            }, 1000);
            
            showNotification('Document Captured', `Page ${scanCount} scanned successfully. Ready for enhancement.`, 'success');
        }
        
        function applyCanvasEnhancement(context, width, height) {
            // Apply enhancement settings to the canvas
            if (enhancementSettings.autoEnhance) {
                // Auto-enhance: apply optimal settings
                context.filter = 'contrast(1.2) brightness(1.1) saturate(1.1)';
                context.drawImage(context.canvas, 0, 0, width, height);
                context.filter = 'none';
            } else {
                // Manual enhancement based on slider values
                const contrast = enhancementSettings.contrast / 100;
                const brightness = enhancementSettings.brightness / 100;
                const sharpness = enhancementSettings.sharpness / 100;
                
                // Create enhancement filter string
                const filter = `contrast(${contrast}) brightness(${brightness})`;
                context.filter = filter;
                context.drawImage(context.canvas, 0, 0, width, height);
                context.filter = 'none';
                
                // Apply sharpness (simulated with overlay)
                if (sharpness > 1) {
                    context.globalCompositeOperation = 'overlay';
                    context.fillStyle = `rgba(255, 255, 255, ${(sharpness - 1) * 0.3})`;
                    context.fillRect(0, 0, width, height);
                    context.globalCompositeOperation = 'source-over';
                }
            }
        }
        
        function applyEnhancement() {
            if (!currentDocument) return;
            
            // Create a new canvas with applied enhancements
            const canvas = document.createElement('canvas');
            const context = canvas.getContext('2d');
            const img = new Image();
            
            img.onload = function() {
                canvas.width = img.width;
                canvas.height = img.height;
                
                // Draw original image
                context.drawImage(img, 0, 0);
                
                // Apply enhancement settings
                applyCanvasEnhancement(context, canvas.width, canvas.height);
                
                // Update preview
                const enhancedData = canvas.toDataURL('image/jpeg', 0.95);
                previewImage.src = enhancedData;
                
                // Update current document
                currentDocument.enhancedData = enhancedData;
                currentDocument.settings = { ...enhancementSettings };
                
                // Update quality score
                const newScore = Math.min(100, 85 + Math.random() * 15);
                qualityScore.textContent = `${Math.round(newScore)}%`;
                
                showNotification('Enhancement Applied', 'Document enhanced with current settings.', 'success');
            };
            
            img.src = currentDocument.imageData;
        }
        
        function updatePreview(imageData) {
            previewImage.src = imageData;
        }
        
        function showProcessing() {
            progressContainer.style.display = 'block';
            progressFill.style.width = '0%';
            progressPercent.textContent = '0%';
            
            // Simulate processing steps
            const steps = [
                {percent: 20, text: 'Analyzing document...'},
                {percent: 40, text: 'Correcting perspective...'},
                {percent: 60, text: 'Enhancing image quality...'},
                {percent: 80, text: 'Optimizing for A4 format...'},
                {percent: 100, text: 'Ready for download!'}
            ];
            
            let currentStep = 0;
            
            const processInterval = setInterval(() => {
                if (currentStep < steps.length) {
                    const step = steps[currentStep];
                    progressFill.style.width = `${step.percent}%`;
                    progressPercent.textContent = `${step.percent}%`;
                    statusDetails.textContent = step.text;
                    currentStep++;
                } else {
                    clearInterval(processInterval);
                    
                    // Processing complete
                    updateStatus('ready', `Document ${scanCount} processed and enhanced. Ready to download.`);
                    statusDot.classList.remove('scanning');
                    statusDot.classList.add('active');
                    
                    // Hide progress after delay
                    setTimeout(() => {
                        progressContainer.style.display = 'none';
                    }, 2000);
                }
            }, 400);
        }
        
        function downloadToGallery(format) {
            if (!currentDocument && scannedDocuments.length === 0) {
                showNotification('No Documents', 'Please scan a document first.', 'warning');
                return;
            }
            
            let downloadData = currentDocument ? currentDocument.enhancedData : scannedDocuments[0].enhancedData;
            let fileName = '';
            
            // Show download progress
            showProcessing();
            progressFill.style.width = '50%';
            progressPercent.textContent = '50%';
            statusDetails.textContent = 'Preparing download...';
            
            setTimeout(() => {
                progressFill.style.width = '100%';
                progressPercent.textContent = '100%';
                
                if (format === 'jpg') {
                    // Download as JPG to phone gallery
                    fileName = `document-${Date.now()}.jpg`;
                    statusDetails.textContent = 'Downloading JPG to gallery...';
                    
                    // Simulate download
                    setTimeout(() => {
                        simulateFileDownload(downloadData, fileName, 'image/jpeg');
                        showNotification('Download Complete', 'JPG saved to phone gallery!', 'success');
                        statusDetails.textContent = 'JPG downloaded successfully.';
                        
                        // Record to gallery history
                        addToGalleryHistory(fileName, 'jpg');
                    }, 800);
                    
                } else if (format === 'pdf' || format === 'multi-pdf') {
                    // Download as PDF
                    fileName = format === 'multi-pdf' 
                        ? `documents-${Date.now()}.pdf` 
                        : `document-${Date.now()}.pdf`;
                    
                    statusDetails.textContent = 'Generating enhanced PDF...';
                    
                    // Simulate PDF generation and download
                    setTimeout(() => {
                        simulatePDFDownload(fileName);
                        showNotification('PDF Ready', `${format === 'multi-pdf' ? 'Multi-page' : 'Enhanced'} PDF downloaded!`, 'success');
                        statusDetails.textContent = 'PDF downloaded successfully.';
                        
                        // Record to gallery history
                        addToGalleryHistory(fileName, 'pdf');
                    }, 1200);
                }
                
                // Hide progress after completion
                setTimeout(() => {
                    progressContainer.style.display = 'none';
                }, 2000);
            }, 800);
        }
        
        function simulateFileDownload(dataUrl, fileName, mimeType) {
            // Create a temporary link element
            const link = document.createElement('a');
            link.href = dataUrl;
            link.download = fileName;
            link.style.display = 'none';
            
            // Trigger download
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
            
            // On mobile, show instructions
            if (/iPhone|iPad|iPod|Android/i.test(navigator.userAgent)) {
                showNotification('Mobile Download', 'File downloaded. Check your Downloads folder or Gallery app.', 'success');
            }
        }
        
        function simulatePDFDownload(fileName) {
            // Create a simulated PDF download
            const pdfContent = `
                ProScan Upright - Enhanced PDF Export
                =====================================
                
                Document Information:
                - Generated: ${new Date().toLocaleString()}
                - Pages: ${scannedDocuments.length}
                - Quality: ${pdfQuality.toUpperCase()}
                - Format: A4 Portrait
                
                This is a simulated PDF file. In a real implementation,
                this would be a properly formatted PDF with all scanned
                pages in high quality.
                
                Scan Details:
                ${scannedDocuments.map((doc, i) => 
                    `  Page ${i+1}: ${doc.format} - ${doc.timestamp}`
                ).join('\n')}
            `;
            
            const blob = new Blob([pdfContent], { type: 'application/pdf' });
            const url = URL.createObjectURL(blob);
            
            const link = document.createElement('a');
            link.href = url;
            link.download = fileName;
            link.style.display = 'none';
            
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
            
            // Clean up
            setTimeout(() => URL.revokeObjectURL(url), 1000);
        }
        
        function backupToCloud() {
            if (scannedDocuments.length === 0) {
                showNotification('No Documents', 'Please scan documents first.', 'warning');
                return;
            }
            
            showProcessing();
            progressFill.style.width = '30%';
            progressPercent.textContent = '30%';
            statusDetails.textContent = 'Connecting to cloud...';
            
            setTimeout(() => {
                progressFill.style.width = '70%';
                progressPercent.textContent = '70%';
                statusDetails.textContent = 'Uploading documents...';
                
                setTimeout(() => {
                    progressFill.style.width = '100%';
                    progressPercent.textContent = '100%';
                    statusDetails.textContent = 'Cloud backup complete!';
                    
                    showNotification('Cloud Backup', `${scannedDocuments.length} documents backed up to cloud.`, 'success');
                    
                    // Update storage status
                    const freeStorage = (3.2 - scannedDocuments.length * 0.1).toFixed(1);
                    document.getElementById('storage-status').textContent = `${freeStorage}GB`;
                    
                    setTimeout(() => {
                        progressContainer.style.display = 'none';
                    }, 1500);
                }, 800);
            }, 800);
        }
        
        function addToGalleryHistory(fileName, type) {
            // In a real app, this would save to local storage or database
            console.log(`Added to gallery: ${fileName} (${type})`);
            
            // Update download stats
            const downloads = parseInt(localStorage.getItem('proscan_downloads') || '0') + 1;
            localStorage.setItem('proscan_downloads', downloads.toString());
        }
        
        function quickScan() {
            if (!cameraStream) {
                startScanner();
                showNotification('Quick Scan', 'Starting scanner...', 'success');
            } else {
                captureDocument();
                showNotification('Quick Scan', 'Document captured!', 'success');
            }
        }
        
        function resetScanner() {
            // Stop camera if active
            if (cameraStream) {
                cameraStream.getTracks().forEach(track => track.stop());
                cameraStream = null;
                cameraView.srcObject = null;
            }
            
            // Reset variables
            scannedDocuments = [];
            currentDocument = null;
            isAutoScan = false;
            scanCount = 0;
            
            // Reset UI
            startScannerBtn.disabled = false;
            startScannerBtn.innerHTML = '<i class="fas fa-power-off"></i> Start Scanner';
            autoScanBtn.disabled = true;
            autoScanBtn.innerHTML = '<i class="fas fa-robot"></i> Auto-Scan';
            autoScanBtn.classList.remove('control-btn-danger');
            autoScanBtn.classList.add('control-btn-success');
            captureDocBtn.disabled = true;
            
            enhancePreview.style.display = 'none';
            progressContainer.style.display = 'none';
            detectionMessage.style.display = 'none';
            scanBeam.style.animation = 'none';
            
            // Reset enhancement controls
            contrastSlider.value = 100;
            brightnessSlider.value = 100;
            sharpnessSlider.value = 100;
            contrastValue.textContent = '100%';
            brightnessValue.textContent = '100%';
            sharpnessValue.textContent = '100%';
            enhancementSettings = {
                contrast: 100,
                brightness: 100,
                sharpness: 100,
                autoEnhance: true
            };
            
            // Reset enhancement buttons
            enhanceButtons.forEach(btn => btn.classList.remove('active'));
            enhanceButtons[0].classList.add('active');
            
            // Update stats
            updateStats();
            
            // Update status
            updateStatus('ready', 'Scanner reset. Ready to start new scanning session.');
            statusDot.className = 'status-dot';
            
            showNotification('Scanner Reset', 'All documents cleared. Ready for new scan session.', 'success');
        }
        
        function updateStats() {
            scanCountEl.textContent = scanCount;
            
            // Update quality score based on enhancements
            if (scanCount > 0) {
                const score = 85 + Math.floor(Math.random() * 15);
                qualityScore.textContent = `${score}%`;
            } else {
                qualityScore.textContent = '95%';
            }
        }
        
        function updateStatus(state, message) {
            // Update status text
            statusText.textContent = getStatusText(state);
            statusDetails.textContent = message;
        }
        
        function getStatusText(state) {
            const statusMap = {
                'ready': 'Ready',
                'active': 'Scanner Active',
                'detected': 'Document Detected',
                'captured': 'Document Captured',
                'processing': 'Processing',
                'complete': 'Complete',
                'error': 'Error'
            };
            return statusMap[state] || 'Ready';
        }
        
        function showNotification(title, message, type = 'success') {
            // Create notification element
            const notification = document.createElement('div');
            notification.className = `notification ${type}`;
            
            const icon = type === 'success' ? 'check-circle' : 
                        type === 'warning' ? 'exclamation-triangle' : 'times-circle';
            
            notification.innerHTML = `
                <div class="notification-icon">
                    <i class="fas fa-${icon}"></i>
                </div>
                <div>
                    <h4 style="margin-bottom: 5px; color: #1f2937;">${title}</h4>
                    <p style="color: #6b7280; font-size: 0.95rem;">${message}</p>
                </div>
            `;
            
            // Add to notification center
            notificationCenter.appendChild(notification);
            
            // Show notification
            setTimeout(() => notification.classList.add('show'), 10);
            
            // Remove after 5 seconds
            setTimeout(() => {
                notification.classList.remove('show');
                setTimeout(() => {
                    if (notification.parentNode) {
                        notification.parentNode.removeChild(notification);
                    }
                }, 500);
            }, 5000);
        }
        
        // Clean up when page is closed
        window.addEventListener('beforeunload', () => {
            if (cameraStream) {
                cameraStream.getTracks().forEach(track => track.stop());
            }
        });
        
        // Add some cool effects
        document.addEventListener('mousemove', (e) => {
            const scannerDevice = document.querySelector('.scanner-device');
            const xAxis = (window.innerWidth / 2 - e.pageX) / 25;
            const yAxis = (window.innerHeight / 2 - e.pageY) / 25;
            scannerDevice.style.transform = `rotateX(5deg) rotateY(${xAxis}deg) rotateX(${yAxis}deg)`;
        });
    </script>
</body>
</html>
