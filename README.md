# the-ammar-method
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Ammar Method</title>
  <link rel="icon" href="https://i.ibb.co/zS0h3Q1/ammar-logo-gold.png">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #0a0a0a;
      color: #fff;
      overflow-x: hidden;
    }
    h1,h2,h3 {
      font-family: 'Playfair Display', serif;
      color: #d4af37;
    }
    /* Hero */
    .hero {
      position: relative;
      height: 100vh;
      background: url('https://i.ibb.co/zS0h3Q1/ammar-logo-gold.png') center/150px no-repeat, linear-gradient(to bottom, #000, #111);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
    }
    .hero h1 {
      font-size: 3.5rem;
      animation: fadeDown 1.2s ease forwards;
    }
    .hero p {
      margin-top: 10px;
      font-size: 1.3rem;
      animation: fadeUp 1.5s ease forwards;
    }
    .btn-gold {
      display: inline-block;
      margin-top: 25px;
      padding: 12px 28px;
      background: #d4af37;
      color: #0a0a0a;
      font-weight: bold;
      text-decoration: none;
      border-radius: 4px;
      transition: all 0.3s ease;
      animation: fadeUp 2s ease forwards;
    }
    .btn-gold:hover {
      background: #b9932f;
      box-shadow: 0 0 10px #d4af37;
    }
    /* Sections */
    section {
      padding: 80px 20px;
      text-align: center;
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 1s ease, transform 1s ease;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    .pillars {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 40px;
    }
    .pillar {
      flex: 1 1 200px;
      background: rgba(255,255,255,0.05);
      padding: 20px;
      border-radius: 8px;
      border: 1px solid rgba(212,175,55,0.5);
      transition: transform 0.3s ease;
    }
    .pillar:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 10px rgba(212,175,55,0.3);
    }
    .cta {
      background: #111;
      padding: 60px 20px;
    }
    /* Animations */
    @keyframes fadeDown {
      from { opacity: 0; transform: translateY(-30px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <!-- HERO -->
  <section class="hero">
    <h1>The Ammar Method</h1>
    <p>Transform your Qur’an journey into a lifestyle</p>
    <a href="#program" class="btn-gold">Explore Program</a>
  </section>

  <!-- ABOUT -->
  <section class="about" id="about">
    <h2>About The Method</h2>
    <p>Metode ini dirancang untuk membantu perjalanan Qur’an kamu menjadi lebih konsisten, menyenangkan, dan bermakna. Menggabungkan hafalan, tilawah, dan review dengan pendekatan fleksibel namun terstruktur.</p>
  </section>

  <!-- PROGRAM -->
  <section class="program" id="program">
    <h2>The 5 Pillars</h2>
    <div class="pillars">
      <div class="pillar">
        <h3>Hafalan</h3>
        <p>Meningkatkan hafalan ayat secara konsisten setiap hari.</p>
      </div>
      <div class="pillar">
        <h3>Tilawah</h3>
        <p>Menjaga hubungan dengan Qur’an melalui bacaan harian.</p>
      </div>
      <div class="pillar">
        <h3>Muraja’ah</h3>
        <p>Review hafalan lama untuk memperkuat ingatan.</p>
      </div>
      <div class="pillar">
        <h3>Konsistensi</h3>
        <p>Membangun kebiasaan dengan ritme yang realistis.</p>
      </div>
      <div class="pillar">
        <h3>Target</h3>
        <p>Menetapkan tujuan mingguan & bulanan untuk progres jelas.</p>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <section class="cta">
    <h2>Ready to Begin?</h2>
    <a href="https://wa.me/6285830820881" class="btn-gold">Join The Program</a>
  </section>

  <script>
    // Reveal sections on scroll
    const sections = document.querySelectorAll("section");
    window.addEventListener("scroll", () => {
      const trigger = window.innerHeight * 0.8;
      sections.forEach(section => {
        const rect = section.getBoundingClientRect();
        if (rect.top < trigger) {
          section.classList.add("visible");
        }
      });
    });
  </script>
</body>
</html>

