<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>132kV Electrical Substation - Components & Working</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, sans-serif; }
  body { background: #f4f6f9; color: #222; line-height: 1.6; }
  .container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }

  header {
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    color: #fff; padding: 40px 0; text-align: center;
  }
  header h1 { font-size: 2.2rem; margin-bottom: 8px; }
  header p { color: #ffd700; font-size: 1.1rem; }

  nav { background: #1b1b1b; position: sticky; top: 0; z-index: 100; }
  nav ul { display: flex; justify-content: center; list-style: none; flex-wrap: wrap; }
  nav ul li a {
    display: block; color: #fff; padding: 14px 20px;
    text-decoration: none; transition: 0.3s;
  }
  nav ul li a:hover { background: #ffd700; color: #000; }

  .section { padding: 50px 0; }
  .alt-bg { background: #ffffff; }
  .section h2 {
    font-size: 1.8rem; color: #0f2027; margin-bottom: 20px;
    border-left: 5px solid #ffd700; padding-left: 12px;
  }

  .component-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px; margin-top: 20px;
  }
  .card {
    background: #fff; border-radius: 10px; padding: 20px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    border-top: 4px solid #ffd700;
    transition: transform 0.3s, box-shadow 0.3s;
  }
  .card:hover { transform: translateY(-6px); box-shadow: 0 10px 20px rgba(0,0,0,0.15); }
  .card h3 { color: #203a43; margin-bottom: 10px; font-size: 1.15rem; }
  .card p { font-size: 0.95rem; margin-bottom: 8px; color: #444; }

  .diagram {
    background: #0f2027; color: #ffd700; padding: 20px;
    border-radius: 8px; overflow-x: auto; font-size: 0.95rem;
    line-height: 1.8; font-family: 'Courier New', monospace;
  }

  footer {
    background: #1b1b1b; color: #ccc; text-align: center;
    padding: 20px 0; font-size: 0.9rem;
  }

  @media (max-width: 600px) {
    header h1 { font-size: 1.5rem; }
    .section h2 { font-size: 1.4rem; }
  }
</style>
</head>
<body>

<header>
  <div class="container">
    <h1>⚡ 132kV Electrical Substation</h1>
    <p>Components and Their Working Principles</p>
  </div>
</header>

<nav>
  <div class="container">
    <ul>
      <li><a href="#intro">Introduction</a></li>
      <li><a href="#components">Components</a></li>
      <li><a href="#diagram">Single Line Diagram</a></li>
      <li><a href="#about">About</a></li>
    </ul>
  </div>
</nav>

<section id="intro" class="section">
  <div class="container">
    <h2>Introduction</h2>
    <p>
      A <strong>132kV substation</strong> is a high-voltage electrical installation
      used to transmit, distribute, and control electrical power. It steps down
      voltage from 132kV to lower levels (33kV / 11kV) for distribution to
      industrial and residential areas. Below we explain each major component
      and its working principle.
    </p>
  </div>
</section>

<section id="components" class="section alt-bg">
  <div class="container">
    <h2>Major Components & Working</h2>
    <div class="component-grid">

      <div class="card">
        <h3>1. Power Transformer</h3>
        <p><strong>Function:</strong> Step down 132kV to 33kV or 11kV.</p>
        <p><strong>Working:</strong> Uses electromagnetic induction between primary
        and secondary windings. When AC flows through the primary coil, it creates
        a changing magnetic flux in the core, inducing voltage in the secondary coil
        proportional to the turns ratio.</p>
      </div>

      <div class="card">
        <h3>2. Circuit Breaker (SF6 / Vacuum)</h3>
        <p><strong>Function:</strong> Protects circuit during fault by opening automatically.</p>
        <p><strong>Working:</strong> Detects fault current via relay, then trips.
        Uses SF6 gas or vacuum to quench the arc formed when contacts separate.</p>
      </div>

      <div class="card">
        <h3>3. Isolator (Disconnector Switch)</h3>
        <p><strong>Function:</strong> Provides visible isolation for maintenance.</p>
        <p><strong>Working:</strong> Manually or motor operated. Must be opened
        only when no current flows (off-load), otherwise dangerous arc occurs.</p>
      </div>

      <div class="card">
        <h3>4. Current Transformer (CT)</h3>
        <p><strong>Function:</strong> Steps down high current to measurable level (e.g., 5A or 1A).</p>
        <p><strong>Working:</strong> Based on transformer principle. Primary is
        connected in series with the line; secondary feeds meters and relays.</p>
      </div>

      <div class="card">
        <h3>5. Potential Transformer (PT/VT)</h3>
        <p><strong>Function:</strong> Steps down high voltage to low voltage (e.g., 110V) for metering & protection.</p>
        <p><strong>Working:</strong> Primary connected in parallel to the line;
        secondary gives proportional low voltage output.</p>
      </div>

      <div class="card">
        <h3>6. Lightning / Surge Arrester</h3>
        <p><strong>Function:</strong> Protects equipment from lightning surges.</p>
        <p><strong>Working:</strong> Uses non-linear resistor (ZnO). Under normal
        voltage it's insulating; during surge it becomes conductive and diverts
        surge to ground.</p>
      </div>

      <div class="card">
        <h3>7. Busbar</h3>
        <p><strong>Function:</strong> Common conducting path connecting multiple circuits.</p>
        <p><strong>Working:</strong> Made of aluminum or copper. Distributes
        power from incoming to outgoing feeders.</p>
      </div>

      <div class="card">
        <h3>8. Protective Relays</h3>
        <p><strong>Function:</strong> Senses abnormal conditions (overcurrent, earth fault, differential).</p>
        <p><strong>Working:</strong> Compares input (from CT/PT) to set value;
        sends trip signal to circuit breaker when fault detected.</p>
      </div>

      <div class="card">
        <h3>9. Battery & DC System</h3>
        <p><strong>Function:</strong> Supplies control power for relays, breakers, and SCADA.</p>
        <p><strong>Working:</strong> 110V/220V DC battery bank with charger.
        Ensures operation even during AC power failure.</p>
      </div>

      <div class="card">
        <h3>10. Earthing / Grounding System</h3>
        <p><strong>Function:</strong> Safety for personnel and equipment.</p>
        <p><strong>Working:</strong> Provides low-resistance path to ground.
        Includes earth mat, rods, and grid conductor buried underground.</p>
      </div>

    </div>
  </div>
</section>

<section id="diagram" class="section">
  <div class="container">
    <h2>Single Line Diagram (SLD)</h2>
    <p>Typical 132kV substation single line diagram flow:</p>
    <pre class="diagram">
  132kV INCOMING LINE
         |
   [ Lightning Arrester ]
         |
      [ Isolator ]
         |
   [ Circuit Breaker ]
         |
      [ CT / PT ]
         |
      [ BUSBAR ]
         |
   [ Power Transformer 132/33kV ]
         |
   [ 33kV BUSBAR ]
         |
   [ Outgoing Feeders -> Distribution ]
    </pre>
  </div>
</section>

<section id="about" class="section alt-bg">
  <div class="container">
    <h2>About This Project</h2>
    <p>
      Yo project electrical engineering students ra professionals ko lagi
      banayeko ho. Yesle 132kV substation ko components ra tinko working
      principle clear garna help garchha.
    </p>
    <p>Developed by: <strong>Timro Naam</strong></p>
  </div>
</section>

<footer>
  <div class="container">
    <p>© 2025 132kV Substation Project | All Rights Reserved</p>
  </div>
</footer>

<script>
  // Smooth scrolling for nav links
  document.querySelectorAll('nav a').forEach(link => {
    link.addEventListener('click', e => {
      e.preventDefault();
      const target = document.querySelector(link.getAttribute('href'));
      if (target) {
        window.scrollTo({
          top: target.offsetTop - 60,
          behavior: 'smooth'
        });
      }
    });
  });

  // Fade-in animation on scroll
  const cards = document.querySelectorAll('.card');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.style.opacity = 1;
        entry.target.style.transform = 'translateY(0)';
      }
    });
  }, { threshold: 0.1 });

  cards.forEach(card => {
    card.style.opacity = 0;
    card.style.transform = 'translateY(30px)';
    card.style.transition = '0.6s ease';
    observer.observe(card);
  });

  console.log("⚡ 132kV Substation Website Loaded Successfully");
</script>

</body>
</html>
