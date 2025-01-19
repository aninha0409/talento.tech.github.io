<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Layout Responsivo - Roxo</title>
  <style>
    /* Reset Básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Arial', sans-serif;
      line-height: 1.6;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
      background: linear-gradient(135deg, #6a11cb, #2575fc);
      color: #fff;
    }

    header {
      background: #5e17eb;
      color: #fff;
      padding: 1rem;
      text-align: center;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
    }

    header h1 {
      font-size: 2rem;
      animation: fadeIn 2s ease-in-out;
    }

    .navbar {
      background: #4a148c;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
    }

    .navbar ul {
      list-style: none;
      display: flex;
      justify-content: center;
      padding: 1rem;
    }

    .navbar li {
      margin: 0 1rem;
    }

    .navbar a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    .navbar a:hover {
      color: #fbc02d;
    }

    .content {
      display: grid;
      grid-template-columns: 1fr;
      gap: 1rem;
      padding: 1rem;
      flex: 1;
    }

    .main-content,
    .sidebar {
      padding: 1rem;
      border-radius: 8px;
      background: rgba(255, 255, 255, 0.1);
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
      animation: slideUp 1s ease;
    }

    .main-content h2 {
      font-size: 1.5rem;
    }

    .sidebar h3 {
      font-size: 1.3rem;
    }

    .sidebar ul {
      list-style: none;
    }

    .sidebar li {
      margin: 0.5rem 0;
    }

    .sidebar a {
      color: #ffd54f;
      text-decoration: none;
      transition: text-shadow 0.3s ease;
    }

    .sidebar a:hover {
      text-shadow: 0 0 5px #ffd54f, 0 0 10px #ffeb3b;
    }

    .footer {
      background: #4a148c;
      color: #fff;
      text-align: center;
      padding: 1rem;
      font-size: 0.9rem;
      box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.3);
    }

    /* Layout Responsivo */
    @media (min-width: 768px) {
      .content {
        grid-template-columns: 2fr 1fr;
      }
    }

    /* Animações */
    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    @keyframes slideUp {
      from {
        transform: translateY(20px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }
  </style>
</head>
<body>
  <header class="header">
    <h1>Bem-vindo Talento Tech!</h1>
  </header>

  <nav class="navbar">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Sobre</a></li>
      <li><a href="#">Serviços</a></li>
      <li><a href="#">Contato</a></li>
    </ul>
  </nav>

  <main class="content">
    <section class="main-content">
      <h2>Bem-vindo!</h2>
      <p>Este layout foi criado com uma paleta de tons roxos vibrantes e animações suaves!</p>
    </section>

    <aside class="sidebar">
      <h3>Links Úteis</h3>
      <ul>
        <li><a href="#">Link 1</a></li>
        <li><a href="#">Link 2</a></li>
        <li><a href="#">Link 3</a></li>
      </ul>
    </aside>
  </main>

  <footer class="footer">
    <p>&copy; Talento Tech 2025.</p>
  </footer>
</body>
</html>
