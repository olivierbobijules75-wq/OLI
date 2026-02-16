<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>OLI'energie - Solutions Énergétiques</title>
    <style>
      body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), 
                    url('https://images.unsplash.com/photo-1509391366360-fe5bb584852a?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
        background-size: cover;
        background-position: center;
        background-attachment: fixed;
        display: flex;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        margin: 0;
        padding: 20px;
      }

      .container {
        background: rgba(255, 255, 255, 0.96);
        padding: 40px;
        border-radius: 20px;
        max-width: 500px;
        width: 100%;
        box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        border-top: 10px solid #28a745;
        backdrop-filter: blur(5px);
      }

      h2 {
        color: #1a2a3a;
        text-align: center;
        margin-bottom: 5px;
        font-size: 26px;
        text-transform: uppercase;
      }

      .subtitle {
        text-align: center;
        color: #28a745;
        margin-bottom: 25px;
        font-size: 14px;
        font-weight: bold;
        letter-spacing: 1px;
      }

      label {
        display: block;
        margin-bottom: 8px;
        font-weight: 600;
      }

      .phone-group {
        display: flex;
        gap: 10px;
        margin-bottom: 20px;
      }

      input, select, textarea {
        width: 100%;
        padding: 12px;
        margin-bottom: 20px;
        border: 2px solid #ddd;
        border-radius: 10px;
        box-sizing: border-box;
      }

      .btn-send {
        background: linear-gradient(135deg, #28a745, #218838);
        color: white;
        padding: 16px;
        border: none;
        border-radius: 10px;
        cursor: pointer;
        width: 100%;
        font-size: 18px;
        font-weight: bold;
        transition: 0.3s;
      }

      .btn-whatsapp {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: #25d366;
        color: white;
        text-decoration: none;
        padding: 12px;
        border-radius: 10px;
        margin-top: 15px;
        font-weight: bold;
        transition: 0.3s;
      }

      .btn-whatsapp:hover {
        background-color: #128c7e;
      }

      .btn-whatsapp img {
        width: 20px;
        margin-right: 10px;
      }
    </style>
</head>
<body>

<div class="container">
    <h2>OLI'energie</h2>
    <p class="subtitle">BIENVENU CHEZ OLI'energie</p>

    <form action="https://formsubmit.co/olivierbobijules75@gmail.com" method="POST">
        <input type="hidden" name="_captcha" value="false">
        
        <label>Nom complet</label>
        <input type="text" name="Nom" placeholder="Votre nom" required>

        <label>Téléphone</label>
        <div class="phone-group">
            <select name="Code" style="flex:1">
                <option value="+243">🇨🇩 +243</option>
                <option value="+33">🇫🇷 +33</option>
                <option value="+225">🇨🇮 +225</option>
            </select>
            <input type="tel" name="Numero" placeholder="Numéro" style="flex:2" required>
        </div>

        <label>Email</label>
        <input type="email" name="Email" placeholder="votre@email.com" required>

        <label>Message</label>
        <textarea name="Message" rows="3"></textarea>

        <button type="submit" class="btn-send">Envoyer par Email</button>
    </form>

    <a href="https://wa.me/243830998296" class="btn-whatsapp" target="_blank">
        Contactez-nous sur WhatsApp
    </a>
</div>

</body>
</html>
