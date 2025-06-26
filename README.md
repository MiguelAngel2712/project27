<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Inauguración Chocolatería Artesanal</title>
  <style>
    /* RESET BÁSICO */
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Playfair Display', serif;
      background-color: #f3ece2;
      color: #3e2c2a;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 2rem;
    }

    main {
      width: 100%;
      max-width: 720px;
    }

    .invite-card {
      position: relative;
      background: #3e2c2a;
      border: 5px solid #d4af37;
      border-radius: 18px;
      overflow: hidden;
      box-shadow: 0 10px 25px rgba(0,0,0,0.4);
    }

    .invite-card::before {
      content: "";
      position: absolute;
      inset: 0;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/6/65/Cocoa_Beans.jpg/1200px-Cocoa_Beans.jpg') center/cover no-repeat;
      opacity: 0.3;
      z-index: 0;
    }

    .content {
      position: relative;
      z-index: 1;
      background: rgba(243, 236, 226, 0.95);
      padding: 3rem 2.5rem;
      text-align: center;
    }

    .content h1 {
      font-size: 2.8rem;
      margin-bottom: 0.5rem;
      color: #3e2c2a;
      letter-spacing: 3px;
    }

    .content h2 {
      font-size: 1.6rem;
      margin-bottom: 1.8rem;
      color: #d4af37;
      font-style: italic;
    }

    .content p {
      font-size: 1.1rem;
      margin-bottom: 1.2rem;
      line-height: 1.5;
    }

    .rsvp-button {
      display: inline-block;
      margin-top: 1.8rem;
      padding: 0.9rem 2.2rem;
      font-size: 1rem;
      font-weight: bold;
      font-family: 'Montserrat', sans-serif;
      color: #f3ece2;
      background-color: #3e2c2a;
      border: 3px solid #d4af37;
      border-radius: 10px;
      text-decoration: none;
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    .rsvp-button:hover {
      background-color: #d4af37;
      color: #3e2c2a;
    }

    .shop-image {
      position: absolute;
      bottom: 1.5rem;
      right: 1.5rem;
      width: 160px;
      border: 5px solid #f3ece2;
      border-radius: 14px;
      object-fit: cover;
      z-index: 1;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
    }

    footer {
      margin-top: 2.5rem;
      font-size: 0.85rem;
      color: #6b5954;
      text-align: center;
      font-style: italic;
    }
  </style>
</head>
<body>

  <main>
    <div class="invite-card" role="region" aria-label="Invitación a la inauguración de Chocolatería Artesanal Dulce Decadencia">
      <div class="content">
        <header>
          <h1>Inauguración Chocolatería Artesanal</h1>
          <h2>Dulce Decadencia</h2>
        </header>
        <p>📅 <strong>15 de julio de 2025</strong> • 17:00</p>
        <p>📍 <strong>Hotel Chocolat</strong>, 58-59 Sloane Avenue, Londres</p>
        <p>Te invitamos a una experiencia sensorial: catas premium, recorrido guiado y obsequios exclusivos.</p>
        <a href="#" class="rsvp-button" aria-label="Confirmar asistencia al evento">Confirmar Asistencia</a>
      </div>
      <img
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Cacao_Fruit_with_Beans.JPG/800px-Cacao_Fruit_with_Beans.JPG"
        alt="Fruto del cacao con granos"
        class="shop-image"
      />
    </div>
  </main>

  <footer>&copy; 2025 Dulce Decadencia. Todos los derechos reservados.</footer>

</body>
</html>
