<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OLI'energie - Solutions Énergétiques Professionnelles</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root {
            --primary-color: #28a745;
            --secondary-color: #1a2a3a;
            --accent-color: #f8f9fa;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(rgba(26, 42, 58, 0.8), rgba(26, 42, 58, 0.8)), 
                        url('https://images.unsplash.com/photo-1509391366360-fe5bb584852a?auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            margin: 0;
            padding: 40px 20px;
            color: #333;
        }

        .main-wrapper {
            max-width: 900px;
            margin: 0 auto;
        }

        /* --- Header & Container --- */
        .container {
            background: rgba(255, 255, 255, 0.98);
            padding: 40px;
            border-radius: 24px;
            box-shadow: 0 25px 50px rgba(0,0,0,0.3);
            border-top: 8px solid var(--primary-color);
        }

        h1 {
            color: var(--secondary-color);
            text-align: center;
            margin: 0;
            font-weight: 800;
            font-size: 32px;
            letter-spacing: -1px;
        }

        .subtitle {
            text-align: center;
            color: var(--primary-color);
            margin-bottom: 30px;
            font-size: 14px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* --- Tableau des Services --- */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }

        .service-card {
            background: var(--accent-color);
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s ease;
            border: 1px solid #eee;
        }

        .service-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary-color);
        }

        .service-card i {
            font-size: 30px;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .service-card h3 {
            margin: 0 0 10px 0;
            font-size: 18px;
            color: var(--secondary-color);
        }

        .service-card p {
            font-size: 14px;
            color: #666;
            margin: 0;
        }

        /* --- Formulaire --- */
        .form-section {
            border-top: 1px solid #eee;
            padding-top: 30px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            font-size: 14px;
        }

        .phone-group {
            display: flex;
            gap: 10px;
        }

        input, select, textarea {
            width: 100%;
            padding: 14px;
            margin-bottom: 20px;
            border: 2px solid #e1e1e1;
            border-radius: 12px;
            font-family: inherit;
            transition: 0.3s;
        }

        input:focus, select:focus, textarea:focus {
            outline: none;
            border-color: var(--primary-color);
            background: #fff;
        }

        .btn-send {
            background: var(--primary-color);
            color: white;
            padding: 18px;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            width: 100%;
            font-size: 16px;
            font-weight: 700;
            transition: 0.3s;
            text-transform: uppercase;
        }

        .btn-send:hover {
            background: #218838;
            box-shadow: 0 10px 20px rgba(40, 167, 69, 0.3);
        }

        .btn-whatsapp {
            display: flex;
            align-items: center;
            justify-content: center;
            background: #25d366;
            color: white;
            text-decoration: none;
            padding: 14px;
            border-radius: 12px;
            margin-top: 15px;
            font-weight: 700;
            transition: 0.3s;
        }

        .btn-whatsapp:hover {
            background: #128c7e;
            transform: scale(1.02);
        }

        .btn-whatsapp i {
            margin-right: 10px;
            font-size: 20px;
        }

        @media (max-width: 600px) {
            .container { padding: 20px; }
            h1 { font-size: 24px; }
        }
    </style>
</head>
<body>

<div class="main-wrapper">
    <div class="container">
        <h1>OLI'energie</h1>
        <p class="subtitle">Expertise en Solutions Énergétiques</p>

        <div class="services-grid">
            <div class="service-card">
                <i class="fas fa-solar-panel"></i>
                <h3>Installation Solaire</h3>
                <p>Pose de panneaux photovoltaïques haute performance.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-battery-full"></i>
                <h3>Maintenance</h3>
                <p>Entretien et optimisation de vos systèmes de stockage.</p>
            </div>
            <div class="service-card">
                <div style="font-size: 30px; color: #28a745; margin-bottom: 15px;">⚡</div>
                <h3>Audit Énergétique</h3>
                <p>Analyse complète pour réduire vos factures.</p>
            </div>
        </div>

        <div class="form-section">
            <form action="https://formsubmit.co/olivierbobijules75@gmail.com" method="POST">
                <input type="hidden" name="_captcha" value="false">
                
                <label><i class="fas fa-user"></i> Nom complet</label>
                <input type="text" name="Nom" placeholder="Ex: Jean Dupont" required>

                <label><i class="fas fa-phone"></i> Téléphone</label>
                <div class="phone-group">
                    <select name="Code" style="flex:1">
                        <option value="+243">🇨🇩 +243</option>
                        <option value="+33">🇫🇷 +33</option>
                        <option value="+225">🇨🇮 +225</option>
                    </select>
                    <input type="tel" name="Numero" placeholder="830998296" style="flex:2" required>
                </div>

                <label><i class="fas fa-envelope"></i> Email professionnel</label>
                <input type="email" name="Email" placeholder="nom@entreprise.com" required>

                <label><i class="fas fa-comment-alt"></i> Détails de votre projet</label>
                <textarea name="Message" rows="3" placeholder="Décrivez vos besoins..."></textarea>

                <button type="submit" class="btn-send">Envoyer la demande d'étude</button>
            </form>

            <a href="https://wa.me/243830998296" class="btn-whatsapp" target="_blank">
                <i class="fab fa-whatsapp"></i> Discuter sur WhatsApp
            </a>
        </div>
    </div>
</div>

</body>
</html>
