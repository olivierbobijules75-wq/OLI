<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OLI'energie - Expertise & Solutions</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root { --primary: #28a745; --dark: #1a2a3a; }

        body {
            font-family: 'Inter', sans-serif;
            background: #f4f7f6;
            margin: 0;
            padding: 0;
        }

        /* --- HEADER & LOGO --- */
        header {
            background: var(--dark);
            padding: 20px;
            text-align: center;
            color: white;
        }
        header h1 span { color: var(--primary); }

        /* --- DIAPORAMA (SLIDER) --- */
        .slider-container {
            width: 100%;
            max-width: 1100px;
            height: 400px;
            margin: 20px auto;
            overflow: hidden;
            border-radius: 20px;
            position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .slides {
            display: flex;
            width: 500%; /* Ajuster selon le nombre de photos */
            height: 100%;
            transition: transform 1s ease-in-out;
        }

        .slides img {
            width: 100%;
            height: 400px;
            object-fit: cover; /* Important pour que les photos gardent une belle forme */
        }

        /* --- MISE EN PAGE PRINCIPALE --- */
        .main-container {
            max-width: 1100px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 30px;
            padding: 20px;
        }

        .services-panel, .form-panel {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .category-title {
            color: var(--primary);
            font-weight: 700;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .service-list {
            list-style: none;
            padding: 0;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
            margin-bottom: 20px;
        }

        /* --- FORMULAIRE --- */
        .form-panel { border-top: 6px solid var(--primary); position: sticky; top: 20px; }
        input, select, textarea { width: 100%; padding: 12px; margin-bottom: 15px; border: 2px solid #eee; border-radius: 10px; box-sizing: border-box; }
        .btn-send { background: var(--primary); color: white; border: none; padding: 15px; width: 100%; border-radius: 10px; font-weight: 700; cursor: pointer; }
        .btn-whatsapp { display: flex; align-items: center; justify-content: center; background: #25d366; color: white; text-decoration: none; padding: 12px; border-radius: 10px; margin-top: 10px; font-weight: 700; }

        @media (max-width: 900px) {
            .main-container { grid-template-columns: 1fr; }
            .slider-container { height: 250px; }
            .slides img { height: 250px; }
        }
    </style>
</head>
<body>

<header>
    <h1>OLI<span>'energie</span></h1>
    <p>Solutions Énergétiques & Services Techniques</p>
</header>

<div class="slider-container">
    <div class="slides" id="slider">
        <img src="me.jpg" alt="Installation Panneaux">
        <img src="PXL_20260120_093002664.MP.jpg" alt="Système Batterie Ragie">
        <img src="PXL_20251030_065834633.jpg" alt="Installation TV & LED">
        <img src="PXL_20250909_073748394.jpg" alt="Installation Starlink">
        <img src="PXL_20250827_173156229.jpg" alt="Tableau Électrique">
    </div>
</div>

<div class="main-container">
    <div class="services-panel">
        <h2>Nos Réalisations & Services</h2>
        
        <div class="category-title"><i class="fas fa-bolt"></i> &nbsp; Électricité & Solaire</div>
        <ul class="service-list">
            <li>Installation Panneaux</li>
            <li>Systèmes Batteries</li>
            <li>Maintenance Inverter</li>
            <li>Réseau SNEL / Groupe</li>
        </ul>

        <div class="category-title"><i class="fas fa-satellite-dish"></i> &nbsp; Antennes & Wi-Fi</div>
        <ul class="service-list">
            <li>Starlink Standard/Mini</li>
            <li>Canal+ / Startimes</li>
            <li>Configuration Wi-Fi</li>
            <li>TNT</li>
        </ul>

        <div class="category-title"><i class="fas fa-tools"></i> &nbsp; Maintenance & Dépannage</div>
        <ul class="service-list">
            <li>Réparation Électronique</li>
            <li>PC & Téléphones</li>
            <li>Maintenance Climatisation</li>
            <li>Montage Supports TV</li>
        </ul>

        <div class="category-title"><i class="fas fa-lightbulb"></i> &nbsp; Décoration LED</div>
        <ul class="service-list">
            <li>Profils LED Design</li>
            <li>Spots Encastrés</li>
            <li>Éclairage Intelligent</li>
        </ul>
    </div>

    <div class="form-panel">
        <h3 style="text-align:center;">Contactez l'expert</h3>
        <form action="https://formsubmit.co/olivierbobijules75@gmail.com" method="POST">
            <input type="hidden" name="_captcha" value="false">
            <input type="text" name="Nom" placeholder="Votre Nom" required>
            
            <div style="display:flex; gap:5px;">
                <select name="Pays" style="flex:1;">
                    <option value="+243">🇨🇩 RDC</option>
                    <option value="+33">🇫🇷 FR</option>
                    <option value="+32">🇧🇪 BE</option>
                </select>
                <input type="tel" name="Numero" placeholder="830998296" style="flex:2;" required>
            </div>

            <select name="Service">
                <option>Solaire / Électricité</option>
                <option>Starlink / Wi-Fi</option>
                <option>Dépannage / Montage</option>
                <option>Décoration LED</option>
            </select>
            <textarea name="Message" rows="3" placeholder="Détails de votre projet..."></textarea>
            <button type="submit" class="btn-send">Envoyer la demande</button>
        </form>
        <a href="https://wa.me/243830998296" class="btn-whatsapp" target="_blank">
            <i class="fab fa-whatsapp"></i>&nbsp; WhatsApp Direct
        </a>
    </div>
</div>

<script>
    let index = 0;
    const slider = document.getElementById('slider');
    const totalSlides = 5; // Nombre de photos

    function nextSlide() {
        index++;
        if (index >= totalSlides) {
            index = 0;
        }
        slider.style.transform = `translateX(-${index * (100 / totalSlides)}%)`;
    }

    // Change de photo toutes les 5000ms (5 secondes)
    setInterval(nextSlide, 5000);
</script>

</body>
</html>
