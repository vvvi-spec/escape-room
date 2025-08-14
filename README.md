<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SecureCam Pro - Villa Bertelli</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: #333;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .header {
            background: rgba(255,255,255,0.95);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            margin-bottom: 30px;
            text-align: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: bold;
            color: #1e3c72;
            margin-bottom: 10px;
        }
        
        .timestamp {
            background: #ff4444;
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-weight: bold;
            display: inline-block;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.7; }
            100% { opacity: 1; }
        }
        
        .camera-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
            margin-bottom: 30px;
        }
        
        .camera-feed {
            background: rgba(255,255,255,0.95);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .camera-feed:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.25);
        }
        
        .camera-header {
            display: flex;
            justify-content: between;
            align-items: center;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid #e0e0e0;
        }
        
        .camera-title {
            font-weight: bold;
            color: #1e3c72;
            font-size: 18px;
        }
        
        .status-indicator {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #4CAF50;
            animation: blink 1.5s infinite;
        }
        
        .status-offline {
            background: #f44336;
            animation: none;
        }
        
        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.3; }
        }
        
        .camera-image {
            width: 100%;
            height: 200px;
            background: #f0f0f0;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 15px;
            position: relative;
            overflow: hidden;
        }
        
        .camera-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border-radius: 10px;
        }
        
        .no-signal {
            color: #666;
            font-style: italic;
            text-align: center;
        }
        
        .camera-details {
            font-size: 14px;
            color: #666;
            line-height: 1.5;
        }
        
        .alibi-section {
            background: rgba(255,255,255,0.95);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
            margin-top: 30px;
        }
        
        .alibi-title {
            font-size: 24px;
            color: #1e3c72;
            margin-bottom: 20px;
            text-align: center;
        }
        
        .person-alibi {
            background: #f8f9fa;
            border-left: 4px solid #4CAF50;
            padding: 15px;
            margin: 15px 0;
            border-radius: 0 10px 10px 0;
        }
        
        .person-name {
            font-weight: bold;
            color: #1e3c72;
            margin-bottom: 5px;
        }
        
        .key-evidence {
            background: linear-gradient(45deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 20px;
            border-radius: 15px;
            margin-top: 30px;
            text-align: center;
            box-shadow: 0 8px 25px rgba(238, 90, 36, 0.3);
        }
        
        .evidence-title {
            font-size: 20px;
            font-weight: bold;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="logo">🔒 SecureCam Pro</div>
            <h2>Sistema di Sicurezza - Villa Bertelli</h2>
            <div class="timestamp">REGISTRAZIONI: 16 Agosto 2025 - 22:30-23:30</div>
        </div>
        
        <div class="camera-grid">
            <div class="camera-feed">
                <div class="camera-header">
                    <div class="camera-title">📹 Lato Destro - Boschetto</div>
                    <div class="status-indicator"></div>
                </div>
                <div class="camera-image">
                    <div style="text-align: center; padding: 20px;">
                        <div style="font-size: 48px; margin-bottom: 10px;">🌳</div>
                        <div><strong>23:00-23:15</strong> - Area sotto osservazione</div>
                        <div style="color: #666; margin-top: 10px;">Nessun movimento rilevato</div>
                        <div style="color: #666;">Zona completamente vuota</div>
                    </div>
                </div>
                <div class="camera-details">
                    <strong>Stato:</strong> Operativo<br>
                    <strong>Ultima attività:</strong> Nessuna<br>
                    <strong>Note:</strong> Area isolata, nessuna presenza
                </div>
            </div>
            
            <div class="camera-feed">
                <div class="camera-header">
                    <div class="camera-title">📹 Retro della Casa</div>
                    <div class="status-indicator"></div>
                </div>
                <div class="camera-image">
                    <div style="text-align: center; padding: 20px;">
                        <div style="font-size: 48px; margin-bottom: 10px;">🏠</div>
                        <div><strong>21:45</strong> - Enrico Bertacchini esce per aria</div>
                        <div style="font-size: 14px; color: #666; margin: 8px 0;">Prende pasticche e usa inalatore per asma</div>
                        <div><strong>23:07</strong> - Area vuota</div>
                    </div>
                </div>
                <div class="camera-details">
                    <strong>Stato:</strong> Operativo<br>
                    <strong>Ultima attività:</strong> 21:45 (Enrico)<br>
                    <strong>Note:</strong> Zona deserta alle 23:07
                </div>
            </div>
            
            <div class="camera-feed">
                <div class="camera-header">
                    <div class="camera-title">📹 Lato Sinistro della Casa</div>
                    <div class="status-indicator"></div>
                </div>
                <div class="camera-image">
                    <div style="text-align: center; padding: 20px;">
                        <div style="font-size: 48px; margin-bottom: 10px;">🏡</div>
                        <div><strong>23:07</strong> - Zona sotto controllo</div>
                        <div style="color: #666; margin-top: 10px;">Niente da rilevare</div>
                        <div style="color: #666;">Nessuna persona nell'area</div>
                    </div>
                </div>
                <div class="camera-details">
                    <strong>Stato:</strong> Operativo<br>
                    <strong>Ultima attività:</strong> Nessuna<br>
                    <strong>Note:</strong> Zona tranquilla, nessun movimento
                </div>
            </div>
            
            <div class="camera-feed">
                <div class="camera-header">
                    <div class="camera-title">📹 Parcheggio e Accesso</div>
                    <div class="status-indicator"></div>
                </div>
                <div class="camera-image">
                    <div style="text-align: center; padding: 20px;">
                        <div style="font-size: 48px; margin-bottom: 10px;">🚗</div>
                        <div><strong>23:05</strong> - Valentina Rossi al parcheggio</div>
                        <div style="font-size: 14px; color: #666; margin: 8px 0;">Va alla macchina a prendere le sigarette</div>
                        <div><strong>23:10</strong> - Torna verso la casa</div>
                        <div style="color: #666; margin-top: 10px;">Movimento documentato alle telecamere</div>
                    </div>
                </div>
                <div class="camera-details">
                    <strong>Stato:</strong> Operativo<br>
                    <strong>Veicoli rilevati:</strong> 6<br>
                    <strong>Note:</strong> Movimento Valentina documentato
                </div>
            </div>
        </div>
        
        
        <div class="key-evidence">
            <div class="evidence-title">🚨 INFORMAZIONI SISTEMA</div>
            <div>Sistema di videosorveglianza esterno attivo. Le telecamere interne sono state disattivate per la privacy degli ospiti durante la festa privata.</div>
        </div>
    </div>
</body>
</html># escape-room
