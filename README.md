<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Acerca de Nosotros - Gab y Santino</title>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      background: linear-gradient(90deg, #a8e063 0%, #56ab2f 100%);
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      min-height: 100vh;
      text-align: center;
      padding: 2rem 1rem;
      position: relative;
      overflow-x: hidden;
    }

    /* Crear el efecto de gradiente direccional */
    body::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: linear-gradient(90deg, 
        rgba(168, 224, 99, 0.9) 0%, 
        rgba(86, 171, 47, 0.9) 100%);
      z-index: -1;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
      animation: fadeInDown 1.5s ease;
    }

    h2 {
      font-size: 1.5rem;
      margin-bottom: 0.3rem;
      color: #d4ffdc;
    }

    .intro {
      font-size: 1.1rem;
      max-width: 600px;
      margin-bottom: 2rem;
      color: rgba(255,255,255,0.9);
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.5rem;
      width: 100%;
      max-width: 900px;
    }

    .card {
      background: rgba(255, 255, 255, 0.15);
      backdrop-filter: blur(8px);
      padding: 1.8rem;
      border-radius: 20px;
      box-shadow: 0 8px 32px rgba(0,0,0,0.3);
      width: 90%;
      max-width: 380px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      animation: fadeInUp 2s ease;
    }

    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 40px rgba(0,0,0,0.4);
    }

    .emoji {
      font-size: 4rem;
      margin-bottom: 1rem;
      display: block;
    }

    p {
      font-size: 1rem;
      color: rgba(255,255,255,0.9);
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 0.8rem;
      margin-top: 2rem;
      width: 90%;
      max-width: 400px;
      background: rgba(255, 255, 255, 0.15);
      padding: 1.5rem;
      border-radius: 15px;
      backdrop-filter: blur(10px);
      box-shadow: 0 4px 20px rgba(0,0,0,0.2);
      animation: fadeIn 2s ease;
    }

    input, textarea, button {
      border: none;
      border-radius: 10px;
      padding: 0.8rem;
      font-size: 1rem;
      width: 100%;
    }

    input, textarea {
      background: rgba(255,255,255,0.2);
      color: #fff;
      outline: none;
    }

    input::placeholder, textarea::placeholder {
      color: rgba(255,255,255,0.7);
    }

    button {
      background: #d4ffdc;
      color: #333;
      font-weight: bold;
      cursor: pointer;
      transition: transform 0.2s, background 0.3s;
    }

    button:hover {
      background: #b3f3b5;
      transform: scale(1.05);
    }

    footer {
      margin-top: 2rem;
      font-size: 0.9rem;
      color: rgba(255,255,255,0.8);
    }

    /* Animaciones */
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(20px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @keyframes fadeInUp {
      from {opacity: 0; transform: translateY(40px);}
      to {opacity: 1; transform: translateY(0);}
    }

    @keyframes fadeInDown {
      from {opacity: 0; transform: translateY(-20px);}
      to {opacity: 1; transform: translateY(0);}
    }
  </style>
</head>
<body>

  <h1>🌿 Acerca de Nosotros</h1>
  <p class="intro">Somos estudiantes de electrónica con diferentes pasiones, pero con algo en común: ¡la curiosidad y las ganas de aprender cada día más! ⚡</p>

  <div class="container">
    <div class="card">
      <span class="emoji">🌱</span>
      <h2>Gabriel Martínez</h2>
      <p>Tengo 19 años, me gusta la alimentacion, la química, la actividad fisica y aprender cosas nuevas.  
      Estoy trabajando en mejorar día a día y convertirme en mi mejor versión 🌱</p>
    </div>

    <div class="card">
      <span class="emoji">🐱</span>
      <h2>Santino Alveal</h2>
      <p>Me apasionan los videojuegos, la tecnología, disfrazarme y tocar el bajo 🎸  
      Siempre busco nuevas formas de expresarme y crecer en el mundo digital.</p>
    </div>
  </div>

  <form>
    <h3>📬 Contáctanos</h3>
    <input type="text" placeholder="Tu nombre" required>
    <input type="email" placeholder="Tu correo electrónico" required>
    <textarea rows="3" placeholder="Tu mensaje..." required></textarea>
    <button type="submit">Enviar</button>
  </form>

  <footer>Hecho con 💚 por Gabriel Martínez & Santino Alveal — 2025</footer>

</body>
</html>
