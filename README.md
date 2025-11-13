<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>OSH Coffee</title>
  <link rel="stylesheet" href="style.css" />
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
    header, nav, footer { text-align: center; padding: 10px; }
    nav ul { list-style: none; padding: 0; }
    nav ul li { display: inline; margin: 0 10px; }
    nav ul li a { text-decoration: none; }
    main { padding: 20px; }
    .hidden { display: none; }
    button { padding: 8px 15px; margin: 10px; cursor: pointer; }
  </style>
</head>
<body>
	
  <video src="assets/kahve2.mp4" autoplay muted></video>
  
  <header>
    <section>
      <h1>D&amp;H</h1><br />
      <h2>Coffee</h2>
    </section>
  </header>
	
  <nav>
    <div id="Nav_Liste">
      <ul>
        <li><button onclick="sayfaGoster('anasayfa')">Anasayfa</button></li>
        <li><button onclick="sayfaGoster('hakkimizda')">Hakkımızda</button></li>
      </ul>
    </div>
  </nav>
	
  <main>
    <!-- Anasayfa -->
    <section id="anasayfa">
      <section id="menuler">
        <div class="menu">
          <h2>Kahve</h2>
          <ul>
            <li>Espresso - 40 TL</li>
            <li>Latte - 45 TL</li>
            <li>Americano - 42 TL</li>
            <li>Mocha - 48 TL</li>
          </ul>
        </div>
				
        <div class="menu">
          <h2>Tatlı</h2>
          <ul>
            <li>Cheesecake - 155 TL</li>
            <li>Brownie - 150 TL</li>
            <li>Profiterol - 150 TL</li>
            <li>Macaron - 250 TL</li>
          </ul>
        </div>
      </section>
    </section>
		
    <!-- Hakkımızda Sayfası -->
    <section id="hakkimizda" class="hidden">
      <h2>Hakkımızda</h2>
      <p>OSH Coffee, 2025 yılında kurulmuş modern bir kahve dükkanıdır. 
         Amacımız misafirlerimize en kaliteli kahveleri ve tatlıları sunmaktır. 
         Her fincanda sevgi ve özenle hazırlanmış bir lezzet bulacaksınız.</p>
    </section>
  </main>
	
  <footer>
    <p>dilarakaymak@gmail.com - 0555 555 5555</p>
    <p>AFİYET OLSUN :)</p>
  </footer>

  <script>
    function sayfaGoster(sayfa) {
      document.getElementById("anasayfa").classList.add("hidden");
      document.getElementById("hakkimizda").classList.add("hidden");
      document.getElementById(sayfa).classList.remove("hidden");
    }
  </script>
</body>
</html>

