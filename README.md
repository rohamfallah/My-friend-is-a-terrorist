# My-friend-is-a-terrorist
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Investigative Summary — 9/11 Interactive</title>
  <style>
    body { font-family: Arial, sans-serif; line-height: 1.6; margin:0; padding:0; background:#f0f0f0; color:#333; }
    header { background:#1a1a1a; color:white; padding:2rem 1rem; text-align:center; }
    main { max-width:900px; margin:2rem auto; background:white; padding:2rem; border-radius:10px; box-shadow:0 4px 20px rgba(0,0,0,0.1);}
    h1, h2 { margin-bottom:1rem; cursor:pointer; }
    section { margin-bottom:1.5rem; }
    ul, ol { margin-left:1.25rem; }
    .callout { background:#fff6d6; padding:1rem; border-left:4px solid #ffd05a; border-radius:6px; }
    footer { text-align:center; color:#666; font-size:0.85rem; margin:2rem 0; }
    a { color:#1a73e8; text-decoration:none; }
    a:hover { text-decoration:underline; }
    .collapsible-content { display:none; padding:0.5rem 0; }
    .timeline { border-left:3px solid #1a73e8; margin:2rem 0; padding-left:1rem; }
    .event { margin-bottom:1rem; position:relative; }
    .event::before { content:''; position:absolute; left:-8px; top:0; width:16px; height:16px; background:#1a73e8; border-radius:50%; }
    .author { font-size:0.9rem; color:#888; margin-top:0.5rem; }
  </style>
</head>
<body>
  <header>
    <h1>Investigative Summary — 9/11 Interactive</h1>
    <p class="author">Created by: Hadi</p>
    <p id="date">Updated: <span></span></p>
  </header>

  <main>
    <section>
      <h2 onclick="toggleSection(this)">Overview ▼</h2>
      <div class="collapsible-content">
        <p>The 9/11 attacks were a series of coordinated terrorist attacks carried out on September 11, 2001. Four commercial airplanes were hijacked, resulting in significant loss of life and property. This summary provides verified information and resources.</p>
      </div>
    </section>

    <section>
      <h2 onclick="toggleSection(this)">Documented Facts ▼</h2>
      <div class="collapsible-content">
        <ul>
          <li><strong>Timeline of Events:</strong> Official timeline by the 9/11 Commission — <a href="https://www.9-11commission.gov/report/911Report.pdf" target="_blank">Read PDF</a></li>
          <li><strong>Casualties & Damage:</strong> Summary by FEMA — <a href="https://www.fema.gov" target="_blank">FEMA Website</a></li>
          <li><strong>Investigations:</strong> 9/11 Commission Report — <a href="https://www.9-11commission.gov/report/911Report.pdf" target="_blank">Official Report</a></li>
        </ul>
      </div>
    </section>

    <section>
      <h2 onclick="toggleSection(this)">Personal Account ▼</h2>
      <div class="collapsible-content">
        <div class="callout">
          <p><em>"This section is for your personal observations or experiences related to the events, without making unverified claims about any individuals."</em></p>
        </div>
      </div>
    </section>

    <section>
      <h2 onclick="toggleSection(this)">Interactive Timeline ▼</h2>
      <div class="collapsible-content timeline">
        <div class="event"><strong>8:46 AM:</strong> Flight 11 crashes into the North Tower of the World Trade Center.</div>
        <div class="event"><strong>9:03 AM:</strong> Flight 175 crashes into the South Tower.</div>
        <div class="event"><strong>9:37 AM:</strong> Flight 77 crashes into the Pentagon.</div>
        <div class="event"><strong>10:03 AM:</strong> Flight 93 crashes in Pennsylvania.</div>
        <div class="event"><strong>10:28 AM:</strong> South Tower collapses.</div>
        <div class="event"><strong>10:30 AM:</strong> North Tower collapses.</div>
      </div>
    </section>

    <section>
      <h2 onclick="toggleSection(this)">Sources & Citations ▼</h2>
      <div class="collapsible-content">
        <ol>
          <li>9/11 Commission Report: <a href="https://www.9-11commission.gov/report/911Report.pdf" target="_blank">Official PDF</a></li>
          <li>FEMA Disaster Reports: <a href="https://www.fema.gov" target="_blank">FEMA Website</a></li>
          <li>National Archives: <a href="https://www.archives.gov/research/9-11" target="_blank">9/11 Records</a></li>
        </ol>
      </div>
    </section>
  </main>

  <footer>
    This site is for informational purposes only. Avoid publishing unverified claims about private individuals.
  </footer>

  <script>
    // Dynamic date
    document.querySelector('#date span').textContent = new Date().toLocaleDateString();

    // Collapsible sections
    function toggleSection(header) {
      const content = header.nextElementSibling;
      if (content.style.display === "block") {
        content.style.display = "none";
        header.textContent = header.textContent.replace('▲','▼');
      } else {
        content.style.display = "block";
        header.textContent = header.textContent.replace('▼','▲');
      }
    }
  </script>
</body>
</html>

