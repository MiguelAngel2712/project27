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
      font-family: Georgia, 'Times New Roman', serif;
      background-color: #faf3e0;
      color: #3b2f2f;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 2rem;
    }

    main {
      width: 100%;
      max-width: 700px;
    }

    .invite-card {
      position: relative;
      background: #3b2f2f;
      border: 4px solid #d4af37;
      border-radius: 16px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    .invite-card::before {
      content: "";
      position: absolute;
      inset: 0;
      background: url('https://cdn.kastatic.org/third_party/javascript-khansrc/live-editor/build/images/food/chocolates.png') center/cover no-repeat;
      opacity: 0.4;
      z-index: 0;
    }

    .content {
      position: relative;
      z-index: 1;
      padding: 3rem 2rem;
      text-align: center;
      background: rgba(250, 243, 224, 0.9);
    }

    .content h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
      color: #3b2f2f;
      letter-spacing: 2px;
    }

    .content h2 {
      font-size: 1.5rem;
      margin-bottom: 1.5rem;
      color: #d4af37;
      font-style: italic;
    }

    .content p {
      font-size: 1.1rem;
      margin-bottom: 1rem;
      line-height: 1.4;
    }

    .rsvp-button {
      display: inline-block;
      margin-top: 1.5rem;
      padding: 0.8rem 2rem;
      font-size: 1rem;
      font-weight: bold;
      color: #faf3e0;
      background-color: #3b2f2f;
      border: 2px solid #d4af37;
      border-radius: 8px;
      text-decoration: none;
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    .rsvp-button:hover {
      background-color: #d4af37;
      color: #3b2f2f;
    }

    .shop-image {
      position: absolute;
      bottom: 1rem;
      right: 1rem;
      width: 140px;
      border: 6px solid #faf3e0;
      border-radius: 12px;
      object-fit: cover;
      z-index: 1;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }

    footer {
      margin-top: 2rem;
      font-size: 0.85rem;
      color: #6b5959;
      text-align: center;
      font-style: italic;
    }
  </style>
</head>
<body>
  <main>
    <div class="invite-card" role="region" aria-label="Invitación a la inauguración de Dulce Decadencia">
      <div class="content">
        <header>
          <h1>Inauguración Chocolatería Artesanal</h1>
          <h2>Dulce Decadencia</h2>
        </header>
        <p>📅 <strong>15 julio 2025</strong>, 17:00</p>
        <p>📍 <strong>Hotel Chocolat</strong>, 58-59 Sloane Avenue, Londres</p>
        <p>Únete a nosotros para una tarde de catas exclusivas, visita guiada y obsequios especiales.</p>
        <form action="/rsvp" method="POST">
          <button type="submit" class="rsvp-button" aria-label="Confirmar asistencia">Confirmar Asistencia</button>
        </form>
      </div>
      <img
        src="https://source.unsplash.com/300x200/?chocolate-shop-london"
        srcset="https://source.unsplash.com/600x400/?chocolate-shop-london 2x"
        alt="Fachada de Hotel Chocolat en Londres"
        class="shop-image"
      />
    </div>
  </main>

  <footer>&copy; 2025 Dulce Decadencia. Todos los derechos reservados.</footer>
</body>
</html>
