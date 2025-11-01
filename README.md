
  <!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Consejo del Día</title>
<style>
  body {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #74ABE2, #5563DE);
    color: #fff;
    text-align: center;
    padding: 40px;
  }
  #contenedor {
    background: rgba(255, 255, 255, 0.15);
    border-radius: 20px;
    padding: 30px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.2);
    transition: transform 0.3s ease-in-out;
  }
  #contenedor:hover {
    transform: scale(1.05);
  }
  p {
    font-size: 1.3em;
    font-weight: 500;
    animation: aparecer 1s ease;
  }
  @keyframes aparecer {
    from {opacity: 0; transform: translateY(20px);}
    to {opacity: 1; transform: translateY(0);}
  }
</style>
</head>
<body>
  <div id="contenedor">
    <h1>💡 Consejo del Día</h1>
    <p id="texto">Cargando...</p>
  </div>

  <script>
    const params = new URLSearchParams(window.location.search);
    const texto = params.get("texto");
    if (texto) {
      document.getElementById("texto").innerText = texto;
    } else {
      document.getElementById("texto").innerText = "Error al cargar consejo.";
    }
  </script>
</body>
</html>

