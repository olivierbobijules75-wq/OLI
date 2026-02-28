<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OLI'energie - Solutions Énergétiques & Services</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #28a745;
            --dark: #1a2a3a;
            --bg-light: #f8f9fa;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(rgba(26, 42, 58, 0.85), rgba(26, 42, 58, 0.85)), 
                        url('https://images.unsplash.com/photo-1621905251189-08b45d6a269e?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            margin: 0;
            padding: 20px;
            color: #333;
        }

        .header-brand {
            text-align: center;
            margin-bottom: 30px;
        }

        .header-brand h1 {
            color: white;
            font-size: 3rem;
            font-weight: 800;
            margin: 0;
            letter-spacing: -1px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .header-brand h1 span { color: var(--primary); }

        .main-container {
            max-width: 1100px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 30px;
            align-items: start;
        }

        .services-panel, .form-panel {
            background: rgba(255, 255, 255, 0.95);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
        }

        .form-panel {
            background: white;
            position: sticky;
            top: 20px;
            border-top: 6px solid var(--primary);
        }

        .category-title {
            display: flex;
            align-items: center;
            color: var(--primary);
            font-size: 1.1rem;
            font-weight: 700;
            margin-bottom: 12px;
        }

        .category-title i {
            margin-right: 12px;
            background: var(--primary);
            color: white;
            padding: 8px;
            border-radius: 8px;
        }

        .service-list {
            list-style: none;
            padding: 0;
            margin: 0 0 20px 0;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 8px;
        }

        .service-list li { font-size: 0.85rem; display: flex; align-items: center; }
        .service-list li::before { content: "•"; color: var(--primary); margin-right: 8px; }

        /* Style du menu des pays */
        .phone-container {
            display: flex;
            gap: 8px;
            margin-bottom: 15px;
        }

        select, input, textarea {
            width: 100%;
            padding: 12px;
            border: 2px solid #edf2f7;
            border-radius: 10px;
            font-family: inherit;
            font-size: 0.9rem;
        }

        .btn-send {
            background: var(--primary);
            color: white;
            padding: 15px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            width: 100%;
            font-weight: 700;
            margin-top: 10px;
        }

        .btn-whatsapp {
            display: flex;
            align-items: center;
            justify-content: center;
            background: #25d366;
            color: white;
            text-decoration: none;
            padding: 12px;
            border-radius: 10px;
            margin-top: 10px;
            font-weight: 700;
        }

        @media (max-width: 900px) {
            .main-container { grid-template-columns: 1fr; }
            .service-list { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

<div class="header-brand">
    <h1>OLI<span>'energie</span></h1>
    <p style="color: white; font-weight: 400;">Solutions Énergétiques & Services Techniques</p>
</div>

<div class="main-container">
    <div class="services-panel">
        <h2 style="margin-top:0;">Nos Services</h2>
        <div class="category-title"><i class="fas fa-bolt"></i> 1. Électricité & Solaire</div>
        <ul class="service-list">
            <li>Batteries & Panneaux</li>
            <li>Groupes électrogènes</li>
            <li>Installation SNEL</li>
            <li>Maintenance réseau</li>
        </ul>

        <div class="category-title"><i class="fas fa-tools"></i> 2. Maintenance Appareils</div>
        <ul class="service-list">
            <li>TV & Radios</li>
            <li>Téléphones & PC</li>
            <li>Décodeurs</li>
            <li>Électroménager</li>
        </ul>

        <div class="category-title"><i class="fas fa-satellite-dish"></i> 3. Antennes & Wi-Fi</div>
        <ul class="service-list">
            <li>Canal+ / Startimes</li>
            <li>Starlink (Tout modèle)</li>
            <li>Médiastar / Zuku</li>
            <li>Configuration Wi-Fi</li>
        </ul>

        <div class="category-title"><i class="fas fa-paint-roller"></i> 4. Montage & Déco</div>
        <ul class="service-list">
            <li>Supports TV muraux</li>
            <li>Climatiseurs</li>
            <li>LED encastrées</li>
            <li>Profils LED Design</li>
        </ul>
    </div>

    <div class="form-panel">
        <h3 style="margin-top:0; text-align:center;">Contactez-nous</h3>
        <form action="https://formsubmit.co/olivierbobijules75@gmail.com" method="POST">
            <input type="hidden" name="_captcha" value="false">
            
            <label style="font-size: 0.8rem; font-weight: 600;">Nom complet</label>
            <input type="text" name="Nom" required style="margin-bottom:15px;">

            <label style="font-size: 0.8rem; font-weight: 600;">Pays & Téléphone</label>
            <div class="phone-container">
                <select name="Pays" style="flex: 1.5; font-size: 0.8rem;">
                    <option value="+243">🇨🇩 RDC (+243)</option>
                    <option value="+33">🇫🇷 France (+33)</option>
                    <option value="+225">🇨🇮 Côte d'Ivoire (+225)</option>
                    <option value="+242">🇨🇬 Congo-Brazza (+242)</option>
                    <option value="+241">🇬🇦 Gabon (+241)</option>
                    <option value="+237">🇨🇲 Cameroun (+237)</option>
                    <option value="+221">🇸🇳 Sénégal (+221)</option>
                    <option value="+212">🇲🇦 Maroc (+212)</option>
                    <option value="+213">🇩🇿 Algérie (+213)</option>
                    <option value="+216">🇹🇳 Tunisie (+216)</option>
                    <option value="+32">🇧🇪 Belgique (+32)</option>
                    <option value="+1">🇺🇸 USA/Canada (+1)</option>
                    <option value="+44">🇬🇧 UK (+44)</option>
                    </select>
                <input type="tel" name="Numero" placeholder="830998296" style="flex: 2;">
            </div>

            <label style="font-size: 0.8rem; font-weight: 600;">Service</label>
            <select name="Service" style="margin-bottom:15px;">
                <option>Solaire / Électricité</option>
                <option>Maintenance / Dépannage</option>
                <option>Antennes / Starlink</option>
                <option>Décoration LED</option>
            </select>

            <textarea name="Message" rows="3" placeholder="Votre message..."></textarea>

            <button type="submit" class="btn-send">Envoyer par Email</button>
        </form>

        <a href="https://wa.me/243830998296" class="btn-whatsapp" target="_blank">
            <i class="fab fa-whatsapp" style="margin-right:10px;"></i> WhatsApp Direct
        </a>
    </div>
</div>

<footer style="text-align:center; color:white; margin-top:30px; font-size:0.8rem; opacity:0.7;">
    &copy; 2026 OLI'energie - Tous droits réservés
</footer>

</body>
</html>
