<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Taj Mahal – A Monument of Eternal Love</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Lato:wght@300;400;700&display=swap" rel="stylesheet"/>
  <style>
    :root {
      --ivory:   #fdf6ec;
      --gold:    #c9a84c;
      --deep:    #1a1209;
      --marble:  #f0e9dc;
      --muted:   #7a6a55;
      --accent:  #8b3a3a;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      background-color: var(--ivory);
      color: var(--deep);
      font-family: 'Lato', sans-serif;
      font-weight: 300;
      line-height: 1.8;
    }

    header {
      position: relative;
      background: linear-gradient(160deg, #1a1209 0%, #3b2a14 60%, #c9a84c22 100%);
      color: var(--ivory);
      text-align: center;
      padding: 80px 24px 60px;
      overflow: hidden;
    }
    header::before {
      content: '';
      position: absolute;
      inset: 0;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/Taj_Mahal_%28Edited%29.jpeg/1280px-Taj_Mahal_%28Edited%29.jpeg') center/cover no-repeat;
      opacity: 0.18;
    }
    header .badge {
      position: relative;
      display: inline-block;
      font-family: 'Lato', sans-serif;
      font-size: 0.72rem;
      letter-spacing: 0.35em;
      text-transform: uppercase;
      color: var(--gold);
      margin-bottom: 16px;
    }
    header h1 {
      position: relative;
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.4rem, 6vw, 4.5rem);
      font-weight: 700;
      line-height: 1.15;
      text-shadow: 0 2px 18px #0008;
    }
    header h1 em {
      font-style: italic;
      color: var(--gold);
    }
    header .subtitle {
      position: relative;
      margin-top: 14px;
      font-size: 1.05rem;
      color: #e8dcc8;
      letter-spacing: 0.04em;
    }
    .gold-line {
      width: 80px;
      height: 2px;
      background: var(--gold);
      margin: 20px auto 0;
      position: relative;
    }

    main {
      max-width: 900px;
      margin: 0 auto;
      padding: 60px 24px 80px;
    }

    .gallery {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: auto auto;
      gap: 12px;
      margin-bottom: 60px;
    }
    .gallery img {
      width: 100%;
      display: block;
      border-radius: 4px;
      box-shadow: 0 6px 30px #0002;
      object-fit: cover;
      transition: transform 0.35s ease, box-shadow 0.35s ease;
    }
    .gallery img:hover {
      transform: scale(1.02);
      box-shadow: 0 12px 40px #0003;
    }
    .gallery .main-img {
      grid-column: 1 / -1;
      height: 380px;
    }
    .gallery .side-img {
      height: 220px;
    }
    figure { display: contents; }

    section { margin-bottom: 52px; }

    h2 {
      font-family: 'Playfair Display', serif;
      font-size: 1.85rem;
      font-weight: 700;
      color: var(--deep);
      margin-bottom: 18px;
      padding-bottom: 10px;
      border-bottom: 1px solid #e0d0bb;
      display: flex;
      align-items: center;
      gap: 12px;
    }
    h2 .num {
      font-family: 'Lato', sans-serif;
      font-size: 0.72rem;
      letter-spacing: 0.22em;
      color: var(--gold);
      font-weight: 700;
      text-transform: uppercase;
    }

    p {
      margin-bottom: 16px;
      color: #3d2f1f;
      font-size: 1.02rem;
    }
    p:last-child { margin-bottom: 0; }

    .facts-box {
      background: linear-gradient(135deg, #3b2a14 0%, #1a1209 100%);
      color: var(--ivory);
      border-radius: 8px;
      padding: 40px 44px;
      position: relative;
      overflow: hidden;
    }
    .facts-box::before {
      content: '✦';
      position: absolute;
      right: 30px;
      top: 18px;
      font-size: 5rem;
      color: #ffffff08;
      pointer-events: none;
    }
    .facts-box h2 {
      color: var(--gold);
      border-bottom-color: #ffffff20;
    }
    .facts-box ul {
      list-style: none;
      padding: 0;
      display: grid;
      gap: 14px;
    }
    .facts-box ul li {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      font-size: 0.97rem;
      line-height: 1.6;
      color: #e8dcc8;
    }
    .facts-box ul li::before {
      content: '◆';
      color: var(--gold);
      font-size: 0.6rem;
      margin-top: 6px;
      flex-shrink: 0;
    }

    blockquote {
      border-left: 3px solid var(--gold);
      margin: 36px 0;
      padding: 18px 28px;
      background: var(--marble);
      border-radius: 0 6px 6px 0;
      font-family: 'Playfair Display', serif;
      font-style: italic;
      font-size: 1.18rem;
      color: var(--accent);
    }
    blockquote cite {
      display: block;
      margin-top: 10px;
      font-style: normal;
      font-family: 'Lato', sans-serif;
      font-size: 0.78rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--muted);
    }

    footer {
      background: var(--deep);
      color: #a08060;
      text-align: center;
      padding: 36px 24px;
      font-size: 0.85rem;
      letter-spacing: 0.04em;
    }
    footer strong {
      color: var(--gold);
      font-weight: 700;
    }
    footer .divider {
      margin: 0 10px;
      opacity: 0.4;
    }

    @media (max-width: 600px) {
      .gallery { grid-template-columns: 1fr; }
      .gallery .main-img { height: 240px; }
      .gallery .side-img { height: 180px; }
      .facts-box { padding: 28px 22px; }
      header { padding: 60px 16px 44px; }
    }
  </style>
</head>
<body>

<header>
  <p class="badge">World Heritage Site &nbsp;·&nbsp; Agra, India</p>
  <h1>The <em>Taj Mahal</em></h1>
  <p class="subtitle">A Monument of Eternal Love &amp; Mughal Splendour</p>
  <div class="gold-line"></div>
</header>

<main>

  <div class="gallery">
    <img class="main-img"
         src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR7FEgcfZ-YLWcHhxGaHkB3i3ImGoi0w7xoieKb0JyuLQ&s=10"
         alt="Taj Mahal front view" />
    <img class="side-img"
         src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRIfYtNwJoL8jbsFnWDkmirReczXnFjiw5DdeZRfCoFJeEzNS6-ZI7dohB_&s=10"
         alt="Taj Mahal view 2" />
    <img class="side-img"
         src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRSC_NiBdL6Q4wH0mkw3-dGxS6sR6h_xhFLSv7yve_NiaGaR0MAviJOatA&s=10"
         alt="Taj Mahal view 3" />
  </div>

  <section>
    <h2><span class="num">01</span> What Is the Taj Mahal?</h2>
    <p>
      The Taj Mahal is one of the world's most iconic and breathtakingly beautiful structures — a
      mausoleum of gleaming white marble that rises above the southern bank of the Yamuna River
      in Agra, India. It stands as the supreme expression of Mughal architecture, seamlessly
      blending Persian, Islamic, and Indian artistic traditions into a single, harmonious whole.
    </p>
    <p>
      Built as a final resting place, the Taj Mahal is more than a tomb — it is a declaration of
      love frozen in stone. Its perfect symmetry, luminous marble that shifts colour with the
      light, and intricately inlaid floral patterns make it a masterpiece unlike anything else
      on earth. Recognised by UNESCO as a World Heritage Site in 1983, it continues to draw
      more than seven million visitors each year.
    </p>
  </section>

  <blockquote>
    "Not a piece of architecture, as other buildings are, but the proud passions of an emperor's
    love wrought in living stones."
    <cite>— Sir Edwin Arnold, Poet</cite>
  </blockquote>

  <section>
    <h2><span class="num">02</span> Location &amp; Construction</h2>
    <p>
      The Taj Mahal is situated in Agra, in the northern Indian state of Uttar Pradesh, approximately
      200 kilometres south of New Delhi. The choice of site — on a bend of the Yamuna — was
      deliberate: the river provides a natural moat and ensures the monument is visible from a
      great distance, especially the north face reflected in the long rectangular pool that
      stretches through the formal garden.
    </p>
    <p>
      Construction began around 1632 CE under the orders of Mughal Emperor Shah Jahan, in memory
      of his beloved wife Mumtaz Mahal, who died during the birth of their fourteenth child.
      The project employed an estimated 20,000 artisans and labourers drawn from across the
      empire and beyond — from Persia, the Ottoman Empire, and Central Asia. The main mausoleum
      was completed by 1643, while the surrounding complex of gardens, gateways, and mosques
      took until approximately 1653 to finish, at a total cost equivalent to billions of
      dollars in today's money.
    </p>
  </section>

  <section>
    <h2><span class="num">03</span> Historical Importance</h2>
    <p>
      The Taj Mahal represents the zenith of Mughal cultural achievement. It synthesised the
      finest craftsmanship of an entire era: master calligraphers inscribed Quranic verses in
      elegant black marble around the archways; gem-cutters set thousands of precious and
      semi-precious stones — lapis lazuli, jade, turquoise, onyx — into the white marble
      in a technique called <em>pietra dura</em>; and architects solved complex engineering
      problems to ensure the four minarets lean slightly outward so they would fall away
      from the main dome in the event of an earthquake.
    </p>
    <p>
      Beyond architecture, the Taj Mahal is a cultural symbol of India itself. It appears on
      banknotes, passports, and in literature across the world. Its image has inspired centuries
      of painters, poets, and travellers. Today it is jointly recognised as one of the
      New Seven Wonders of the World (2007), cementing its status as a global heritage
      belonging to all of humanity.
    </p>
  </section>

  <section>
    <div class="facts-box">
      <h2><span class="num" style="color:#c9a84c88">✦</span> Interesting Facts</h2>
      <ul>
        <li>The white marble was quarried in Makrana, Rajasthan, and transported over 300 km to Agra using a fleet of 1,000 elephants.</li>
        <li>The Taj Mahal appears to change colour throughout the day — pinkish at dawn, dazzling white at noon, and golden under moonlight.</li>
        <li>The four minarets are each slightly tilted outward by design, a brilliant earthquake-proofing technique from the 17th century.</li>
        <li>Shah Jahan was later imprisoned by his own son Aurangzeb and spent his final years gazing at the Taj Mahal from the Agra Fort across the river.</li>
        <li>Over 28 types of precious and semi-precious stones from across Asia and Europe were used in the inlay decorations.</li>
        <li>The main dome is 73 metres (240 ft) tall — roughly the height of a 22-storey building.</li>
        <li>During World War II and the 1971 India–Pakistan war, scaffolding was erected around the dome to camouflage the monument from aerial attack.</li>
      </ul>
    </div>
  </section>

</main>

<footer>
  <p>
    <strong>Historical Place Assignment</strong>
    <span class="divider">|</span>
    Submitted by <strong style="color:#b8860b;">Amruta Rokade</strong>
  </p>
</footer>

</body>
</html>
