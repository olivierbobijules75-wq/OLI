<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solutions Énergétiques & Services Techniques</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
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

        .main-container {
            max-width: 1100px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1.5fr 1fr; /* Services à gauche, Formulaire à droite */
            gap: 30px;
            align-items: start;
        }

        /* --- STYLE DES SERVICES (GAUCHE) --- */
        .services-panel {
            background: rgba(255, 255, 255, 0.95);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
        }

        .service-category {
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 1px solid #eee;
        }

        .service-category:last-child { border: none; }

        .category-title {
            display: flex;
            align-items: center;
            color: var(--primary);
            font-size: 1.2rem;
            font-weight: 700;
            margin-bottom: 12px;
        }

        .category-title i {
            margin-right: 12px;
            background: var(--primary);
            color: white;
            padding: 8px;
            border-radius: 8px;
            font-size: 1rem;
        }

        .service-list {
            list-style: none;
            padding: 0;
            margin: 0;
            display: grid;
            grid-template-columns: 1fr 1fr; /* Sous-listes en 2 colonnes */
            gap: 10px;
        }

        .service-list li {
            font-size: 0.9rem;
            color: #555;
            display: flex;
            align-items: center;
        }

        .service-list li::before {
            content: "•";
            color: var(--primary);
            font-weight: bold;
            margin-right: 8px;
        }

        .sub-category {
            font-weight: 600;
            color: var(--dark);
            margin: 8px 0 5px 0;
            font-size: 0.85rem;
            text-transform: uppercase;
        }

        /* --- STYLE DU FORMULAIRE (DROITE) --- */
        .form-panel {
            background: white;
            padding: 30px;
            border-radius: 20px;
            position: sticky;
            top: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.2);
            border-top: 6px solid var(--primary);
        }

        .form-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 20px;
            text-align: center;
            color: var(--dark);
        }

        label { display: block; margin-bottom: 5px; font-weight: 600; font-size: 0.85rem; }

        input, select, textarea {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            border: 2px solid #edf2f7;
            border-radius: 10px;
            box-sizing: border-box;
            font-family: inherit;
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
            transition: 0.3s;
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
            font-size: 0.9rem;
        }

        /* --- RESPONSIVE --- */
        @media (max-width: 900px) {
            .main-container { grid-template-columns: 1fr; }
            .form-panel { position: static; }
            .service-list { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

<div class="main-container">
    
    <div class="services-panel">
        <h2 style="margin-top:0; color:var(--dark);">Nos Services</h2>

        <div class="service-category">
            <div class="category-title"><i class="fas fa-bolt"></i> 1. Installation électrique</div>
            <div class="sub-category">Courant continu</div>
            <ul class="service-list">
                <li>Batteries</li>
                <li>Panneaux solaires</li>
            </ul>
            <div class="sub-category">Courant alternatif</div>
            <ul class="service-list">
                <li>SNEL</li>
                <li>Groupes électrogènes</li>
            </ul>
        </div>

        <div class="service-category">
            <div class="category-title"><i class="fas fa-tools"></i> 2. Maintenance & Dépannage</div>
            <ul class="service-list">
                <li>Réinstallation & Entretien</li>
                <li>Téléviseurs</li>
                <li>Radios</li>
                <li>Téléphones</li>
                <li>Décodeurs</li>
                <li>Ordinateurs</li>
            </ul>
        </div>

        <div class="service-category">
            <div class="category-title"><i class="fas fa-satellite-dish"></i> 3. Antennes, TNT & Wi-Fi</div>
            <ul class="service-list">
                <li>Canal+ / Startimes</li>
                <li>Euro Star / New World TV</li>
                <li>Médiastar / Zuku Zone</li>
                <li>Starlink (Mini & Standard)</li>
            </ul>
        </div>

        <div class="service-category">
            <div class="category-title"><i class="fas fa-tv"></i> 4. Montage d'équipements</div>
            <ul class="service-list">
                <li>Supports TV muraux</li>
                <li>Climatiseurs</li>
                <li>Autres appareils</li>
            </ul>
        </div>

        <div class="service-category">
            <div class="category-title"><i class="fas fa-lightbulb"></i> 5. Décoration intérieure</div>
            <ul class="service-list">
                <li>Lumières LED encastrées</li>
                <li>Spots lumineux</li>
                <li>Profils LED personnalisés</li>
            </ul>
        </div>
    </div>

    <div class="form-panel">
        <div class="form-title">Demander une intervention</div>
        <form action="https://formsubmit.co/olivierbobijules75@gmail.com" method="POST">
            <input type="hidden" name="_captcha" value="false">
            
            <label>Votre Nom</label>
            <input type="text" name="Nom" required>

            <label>Téléphone (+243)</label>
            <input type="tel" name="Numero" placeholder="830998296" required>

            <label>Service souhaité</label>
            <select name="Service">
                <option>Installation Solaire / Électricité</option>
                <option>Dépannage / Maintenance</option>
                <option>Antenne / Starlink</option>
                <option>Décoration LED</option>
            </select>

            <label>Détails</label>
            <textarea name="Message" rows="3"></textarea>

            <button type="submit" class="btn-send">Envoyer la demande</button>
        </form>

        <a href="https://wa.me/243830998296" class="btn-whatsapp" target="_blank">
            <i class="fab fa-whatsapp" style="margin-right:10px;"></i> WhatsApp : +243 830 998 296
        </a>
    </div>

</div>

</body>
</html>
