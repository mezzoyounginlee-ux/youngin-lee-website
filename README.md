<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Youngin Lee — Mezzo-Soprano</title>
<meta name="description" content="Youngin Lee — Korean Mezzo-Soprano based in Rotterdam, active in opera, concert repertoire and professional ensemble singing across Europe.">
<style>
:root {
  --bg-color: #0b0c10;
  --card-bg: #12141c;
  --text-color: #e0e0e0;
  --text-muted: #999999;
  --accent-gold: #c5a059;
  --accent-gold-light: #e5c178;
  --line-color: rgba(197, 160, 89, 0.2);
  --font-serif: 'Georgia', 'Times New Roman', serif;
  --font-sans: Arial, Helvetica, sans-serif;
}

* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body {
  background-color: var(--bg-color);
  color: var(--text-color);
  font-family: var(--font-sans);
  line-height: 1.6;
  font-weight: 300;
}

a { color: inherit; text-decoration: none; }

/* Navigation */
header {
  position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.8rem 5vw;
  background: rgba(11, 12, 16, 0.92);
  backdrop-filter: blur(10px);
  z-index: 1000;
  border-bottom: 1px solid var(--line-color);
}

.logo {
  font-family: var(--font-serif);
  font-size: 1.5rem;
  letter-spacing: 2px;
  color: #fff;
  text-transform: uppercase;
}

.logo span {
  display: block;
  font-size: 0.7rem;
  letter-spacing: 4px;
  color: var(--accent-gold);
  font-family: var(--font-sans);
}

.right-nav { display: flex; align-items: center; gap: 2rem; }
nav ul { display: flex; list-style: none; gap: 2rem; }
nav a {
  color: var(--text-muted);
  font-size: 0.8rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  transition: color 0.3s;
}
nav a:hover { color: var(--accent-gold); }

.langs { display: flex; gap: 8px; font-size: 0.75rem; letter-spacing: 1px; }
.lang-btn {
  border: none;
  background: none;
  color: var(--text-muted);
  cursor: pointer;
  padding: 2px 4px;
}
.lang-btn.active { color: var(--accent-gold); font-weight: bold; border-bottom: 1px solid var(--accent-gold); }

/* Main Section Layout (Wide Format) */
main { 
  margin-top: 100px; 
  padding: 4rem 4vw 6rem; 
  max-width: 1600px; /* 데스크톱 화면에서 넓게 확장 */
  margin-left: auto; 
  margin-right: auto; 
}
section { margin-bottom: 7rem; scroll-margin-top: 120px; }

.section-title {
  font-family: var(--font-serif);
  font-size: 2.8rem;
  font-weight: 400;
  color: var(--accent-gold);
  margin-bottom: 2.5rem;
  border-bottom: 1px solid var(--line-color);
  padding-bottom: 0.8rem;
}

.sub-header {
  font-family: var(--font-serif);
  font-size: 1.8rem;
  color: #fff;
  margin: 3.5rem 0 1.5rem;
  border-left: 3px solid var(--accent-gold);
  padding-left: 1rem;
}

/* 1. BIOGRAPHY (Wide Layout) */
.bio-container { 
  display: grid; 
  grid-template-columns: 380px 1fr; /* 사진 비율 확대 */
  gap: 4rem; 
  align-items: start; 
}
.photo-placeholder {
  width: 100%;
  height: 500px; /* 세로 높이 확장 */
  border: 1px solid var(--accent-gold);
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--accent-gold);
  letter-spacing: 2px;
  font-size: 0.85rem;
  background: rgba(197, 160, 89, 0.03);
}

.bio-text p { margin-bottom: 1.3rem; color: #ccc; font-size: 1rem; line-height: 1.7; }
.cv-download {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.8rem 2rem;
  border: 1px solid var(--accent-gold);
  color: var(--accent-gold);
  letter-spacing: 2px;
  font-size: 0.8rem;
  text-transform: uppercase;
  transition: 0.3s;
}
.cv-download:hover { background: var(--accent-gold); color: var(--bg-color); }

/* Education Stack */
.edu-list { display: flex; flex-direction: column; gap: 1rem; margin-top: 1rem; }
.edu-item {
  background: var(--card-bg);
  padding: 1.4rem 1.8rem;
  border-left: 2px solid var(--accent-gold);
}
.edu-tag { font-size: 0.75rem; color: var(--accent-gold); letter-spacing: 2px; text-transform: uppercase; }
.edu-degree { font-family: var(--font-serif); font-size: 1.25rem; color: #fff; margin: 0.2rem 0; }
.edu-school { font-size: 0.9rem; color: var(--text-muted); }

/* Integrated Roles & Repertoire */
.rep-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(400px, 1fr)); gap: 2rem; margin-top: 1.5rem; }
.rep-box { background: var(--card-bg); padding: 2.2rem; border: 1px solid rgba(255,255,255,0.05); }
.rep-box h3 { color: var(--accent-gold); margin-bottom: 1.2rem; font-size: 1.35rem; font-family: var(--font-serif); }
.rep-box ul { list-style: none; }
.rep-box li { font-size: 0.95rem; margin-bottom: 0.8rem; color: #bbb; border-bottom: 1px solid rgba(255,255,255,0.03); padding-bottom: 0.4rem; }

/* Collaborators & Press */
.collab-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; background: var(--card-bg); padding: 2.2rem; }
.collab-box h4 { color: var(--accent-gold); font-size: 0.85rem; letter-spacing: 1px; text-transform: uppercase; margin-bottom: 0.5rem; }
.collab-box p { font-size: 0.9rem; color: #bbb; }

.press-quote {
  background: var(--card-bg);
  border-left: 3px solid var(--accent-gold);
  padding: 1.8rem 2.2rem;
  margin-bottom: 1rem;
  font-style: italic;
}
.press-quote p { font-family: var(--font-serif); font-size: 1.15rem; color: #e0e0e0; }
.press-quote span { display: block; font-style: normal; font-size: 0.85rem; color: var(--accent-gold); margin-top: 0.5rem; }

/* 2. AGENDA & ARCHIVE (Vertical Continuous Scroll) */
.year-marker {
  font-family: var(--font-serif);
  font-size: 2.2rem;
  color: var(--accent-gold);
  margin: 2.5rem 0 1rem;
  border-bottom: 1px dashed var(--line-color);
  padding-bottom: 0.3rem;
}

.event-card {
  background: var(--card-bg);
  border-left: 3px solid var(--accent-gold);
  padding: 1.4rem 2rem;
  margin-bottom: 1rem;
  display: grid;
  grid-template-columns: 160px 1fr;
  gap: 1.5rem;
  align-items: center;
}
.event-card.past { opacity: 0.75; border-left-color: #555; }
.event-card.past .event-date { color: #aaa; }
.event-date { color: var(--accent-gold); font-family: var(--font-serif); font-size: 1.25rem; }
.event-details h4 { color: #fff; font-size: 1.1rem; font-weight: 400; }
.event-details p { color: var(--text-muted); font-size: 0.9rem; }

/* 3. MEDIA */
.media-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(450px, 1fr)); gap: 2rem; }
.media-card {
  height: 280px;
  background: var(--card-bg);
  border: 1px dashed var(--line-color);
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--text-muted);
}

/* 4. CONTACT */
.contact-container { display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; }
.contact-info p { margin-bottom: 1rem; font-size: 1rem; }
.contact-info strong { color: var(--accent-gold); font-weight: 400; }

form input, form textarea {
  width: 100%;
  padding: 1rem;
  background: var(--card-bg);
  border: 1px solid rgba(255,255,255,0.1);
  color: #fff;
  margin-bottom: 1rem;
  font-family: var(--font-sans);
  font-size: 0.95rem;
}
form button {
  width: 100%;
  padding: 1rem;
  background: var(--accent-gold);
  border: none;
  color: var(--bg-color);
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  cursor: pointer;
  transition: 0.3s;
}
form button:hover { background: var(--accent-gold-light); }

footer {
  text-align: center;
  padding: 3rem 0;
  border-top: 1px solid var(--line-color);
  color: var(--text-muted);
  font-size: 0.8rem;
  letter-spacing: 2px;
}

@media (max-width: 900px) {
  header { padding: 1.2rem; flex-direction: column; gap: 1rem; }
  main { padding: 1.5rem 4vw; margin-top: 150px; }
  .bio-container, .contact-container { grid-template-columns: 1fr; }
  .rep-grid, .media-grid { grid-template-columns: 1fr; }
  .event-card { grid-template-columns: 1fr; gap: 0.5rem; }
}
</style>
</head>
<body>

<header>
  <a href="#" class="logo">
    Youngin Lee
    <span>Mezzo-Soprano</span>
  </a>
  <div class="right-nav">
    <nav>
      <ul>
        <li><a href="#bio" data-i18n="navBio">Biography</a></li>
        <li><a href="#agenda" data-i18n="navAgenda">Agenda & Archive</a></li>
        <li><a href="#media" data-i18n="navMedia">Media</a></li>
        <li><a href="#contact" data-i18n="navContact">Contact</a></li>
      </ul>
    </nav>
    <div class="langs">
      <button class="lang-btn active" onclick="setLanguage('en')">EN</button>
      <button class="lang-btn" onclick="setLanguage('de')">DE</button>
      <button class="lang-btn" onclick="setLanguage('ko')">KO</button>
    </div>
  </div>
</header>

<main>

  <!-- 1. BIOGRAPHY & REPERTOIRE -->
  <section id="bio">
    <h2 class="section-title" data-i18n="bioTitle">Biography</h2>
    <div class="bio-container">
      <div class="photo-placeholder">
        [ PORTRAIT PHOTO ]
      </div>
      <div class="bio-text">
        <p data-i18n="bioP1">Korean mezzo-soprano <strong>Youngin Lee</strong> is recognized for her dark, warm timbre and deep musical intelligence. Based in Rotterdam, Netherlands, she performs across Europe in opera, oratorio, and professional ensemble projects.</p>
        <p data-i18n="bioP2">Her active professional chorus engagements include the <strong>Dutch National Opera & Ballet</strong> (since 2025/26) and <strong>Groot Omroepkoor</strong> (since 2026/27) as a freelance first alto, along with participation in <strong>NKK NXT</strong> (Nederlands Kamerkoor) and her previous tenure as a Choir Academy Singer at the <strong>Wiener Staatsoper</strong> (2023/24).</p>
        <p data-i18n="bioP3">Lee completed her academic formation across Korea and Germany. She holds a Bachelor of Music in Voice and a Master of Music in Musicology from Ewha Womans University, followed by a Master of Music in Opera from HfM Hanns Eisler Berlin under KS. Dr. Prof. Ewa Wolak. She was honored with the Deutschlandstipendium (2022/23), 1st Prize at the Gold International Classical Music Competition (2025), and Platinum Award at the Global Young Musicians Competition (2025).</p>
        
        <a href="#" class="cv-download" data-i18n="downloadCv">Download Full CV (PDF)</a>
      </div>
    </div>

    <!-- Academic Formation -->
    <h3 class="sub-header" data-i18n="eduHeader">Education & Degrees</h3>
    <div class="edu-list">
      <div class="edu-item">
        <div class="edu-tag" data-i18n="deg1Tag">Bachelor Degree</div>
        <div class="edu-degree" data-i18n="deg1Name">B.M. in Voice (Vocal Performance)</div>
        <div class="edu-school">Ewha Womans University, Seoul — Prof. Mija Park</div>
      </div>
      <div class="edu-item">
        <div class="edu-tag" data-i18n="deg2Tag">Master Degree 1</div>
        <div class="edu-degree" data-i18n="deg2Name">M.M. in Opera</div>
        <div class="edu-school">HfM Hanns Eisler Berlin — KS. Dr. Prof. Ewa Wolak</div>
      </div>
      <div class="edu-item">
        <div class="edu-tag" data-i18n="deg3Tag">Master Degree 2</div>
        <div class="edu-degree" data-i18n="deg3Name">M.M. in Musicology</div>
        <div class="edu-school">Ewha Womans University, Seoul — Prof. Mija Park</div>
      </div>
    </div>

    <!-- Integrated Repertoire & Roles -->
    <h3 class="sub-header" data-i18n="repHeader">Repertoire & Roles</h3>
    <div class="rep-grid">
      <div class="rep-box">
        <h3 data-i18n="repOperaTitle">Opera Roles</h3>
        <ul>
          <li><strong>Dorabella</strong> — W. A. Mozart: <em>Così fan tutte</em></li>
          <li><strong>Dido</strong> — H. Purcell: <em>Dido and Æneas</em></li>
          <li><strong>Hänsel</strong> — E. Humperdinck: <em>Hänsel und Gretel</em></li>
          <li><strong>Cherubino</strong> — W. A. Mozart: <em>Le Nozze di Figaro</em></li>
          <li><strong>L'enfant</strong> — M. Ravel: <em>L'enfant et les sortilèges</em></li>
          <li><strong>Ava</strong> — <em>D:\Faced</em> (World Premiere at Deutsche Oper Berlin)</li>
          <li><strong>Meg</strong> — M. Adamo: <em>Little Women</em></li>
          <li><strong>Charlotte</strong> — J. Massenet: <em>Werther</em></li>
          <li><strong>Idamante</strong> — W. A. Mozart: <em>Idomeneo</em></li>
          <li><strong>3. Dame</strong> — W. A. Mozart: <em>Die Zauberflöte</em></li>
        </ul>
      </div>

      <div class="rep-box">
        <h3 data-i18n="repSacredTitle">Oratorio & Sacred Repertoire</h3>
        <ul>
          <li><strong>J. S. Bach</strong> — Mass in B minor, BWV 232</li>
          <li><strong>J. S. Bach</strong> — Cantata <em>Gelobet sei der Herr, mein Gott</em>, BWV 129</li>
          <li><strong>W. A. Mozart</strong> — Great Mass in C minor, K. 427</li>
          <li><strong>G. Pergolesi</strong> — Missa S. Emidio, P. 47</li>
        </ul>
      </div>
    </div>

    <!-- Artistic Collaborators -->
    <h3 class="sub-header" data-i18n="collabHeader">Artistic Collaborators</h3>
    <div class="collab-grid">
      <div class="collab-box">
        <h4 data-i18n="c1">Conductors</h4>
        <p>Toby Purser, Darijan Ivezic, Michael Lessky, Peter Meiser</p>
      </div>
      <div class="collab-box">
        <h4 data-i18n="c2">Stage Directors</h4>
        <p>Mara Kurotschka, Taro Morikawa, Rebekah Rota, Zsofia Gereb</p>
      </div>
      <div class="collab-box">
        <h4 data-i18n="c3">Music Coaches</h4>
        <p>Andrea Baiocchi, Byron Knutson, Stewart Emerson, Matthias Samuil</p>
      </div>
      <div class="collab-box">
        <h4 data-i18n="c4">Masterclasses</h4>
        <p>Thomas Quasthoff, Mitsuko Shirai, Victoria Loukianetz, Janet Williams, Thomas Guggeis, Peter Berne</p>
      </div>
    </div>

    <!-- Press & Reviews Placeholder -->
    <h3 class="sub-header" data-i18n="pressHeader">Press & Reviews</h3>
    <div class="press-quote">
      <p>"...A mezzo-soprano voice of remarkable warmth, depth, and expressive agility..."</p>
      <span>— European Classical Review</span>
    </div>
  </section>

  <!-- 2. AGENDA & ARCHIVE (Combined Vertical Timeline) -->
  <section id="agenda">
    <h2 class="section-title" data-i18n="agendaTitle">Agenda & Archive</h2>

    <!-- Upcoming 2026+ -->
    <div class="year-marker">2026 — Upcoming</div>
    <div class="event-card">
      <div class="event-date">07 / 2026</div>
      <div class="event-details">
        <h4>Tuingracht Concert</h4>
        <p>Kleurrijk, De Rijp, Netherlands</p>
      </div>
    </div>

    <!-- Archive 2025 -->
    <div class="year-marker">2025</div>
    <div class="event-card past">
      <div class="event-date">12 / 2025</div>
      <div class="event-details">
        <h4>Performance Honoring Korean War Veterans</h4>
        <p>Embassy of South Korea, Den Haag, Netherlands</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">07 / 2025</div>
      <div class="event-details">
        <h4>Yi Jun Commemoration Concert</h4>
        <p>Yi Jun Peace Museum, Den Haag, Netherlands</p>
      </div>
    </div>

    <!-- Archive 2024 -->
    <div class="year-marker">2024</div>
    <div class="event-card past">
      <div class="event-date">12 / 2024</div>
      <div class="event-details">
        <h4>The Netherlands Korean Year-End Concert</h4>
        <p>Postillion Hotel, Amsterdam, Netherlands</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">08 / 2024</div>
      <div class="event-details">
        <h4>Jan Janszn. Weltevree / Pak Yon Commemoration</h4>
        <p>Grote Kerk, De Rijp, Alkmaar, Netherlands</p>
      </div>
    </div>

    <!-- Archive 2023 -->
    <div class="year-marker">2023</div>
    <div class="event-card past">
      <div class="event-date">12 / 2023</div>
      <div class="event-details">
        <h4>G. Pergolesi — Missa S. Emidio, P.47</h4>
        <p>Pfarre Kagran / Franziskanerkirche, Vienna, Austria</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">10 / 2023</div>
      <div class="event-details">
        <h4>Mozart: Così fan tutte (Dorabella) & Ravel: L'enfant et les sortilèges</h4>
        <p>HfM Hanns Eisler Berlin, Germany</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">08 & 09 / 2023</div>
      <div class="event-details">
        <h4>Purcell: Dido and Æneas (Dido)</h4>
        <p>Varaždin National Theater, Croatia</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">07 / 2023</div>
      <div class="event-details">
        <h4>J. S. Bach — Mass in B minor, BWV 232</h4>
        <p>Alte Pfarrkirche Zu den Vier Evangelisten Pankow, Berlin, Germany</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">04 / 2023</div>
      <div class="event-details">
        <h4>D:\Faced [World Premiere] — (Ava)</h4>
        <p>Deutsche Oper Berlin Tischlerei, Germany</p>
      </div>
    </div>

    <!-- Archive 2022 -->
    <div class="year-marker">2022</div>
    <div class="event-card past">
      <div class="event-date">08 / 2022</div>
      <div class="event-details">
        <h4>Mozart: Le Nozze di Figaro (Cherubino)</h4>
        <p>Varaždin National Theater, Croatia</p>
      </div>
    </div>
    <div class="event-card past">
      <div class="event-date">06 / 2022</div>
      <div class="event-details">
        <h4>R. Schumann — Frauenliebe und Leben, Op. 42</h4>
        <p>Schumann Fest Zwickau, Germany</p>
      </div>
    </div>
  </section>

  <!-- 3. MEDIA -->
  <section id="media">
    <h2 class="section-title" data-i18n="mediaTitle">Media</h2>
    <div class="media-grid">
      <div class="media-card">[ Video Embed 1 — Opera Aria ]</div>
      <div class="media-card">[ Video Embed 2 — Lied / Concert ]</div>
    </div>
  </section>

  <!-- 4. CONTACT -->
  <section id="contact">
    <h2 class="section-title" data-i18n="contactTitle">Let's work together.</h2>
    <div class="contact-container">
      <div class="contact-info">
        <p><strong>Location:</strong> Rotterdam, Netherlands</p>
        <p><strong>Email:</strong> mezzo.youngin.lee@gmail.com</p>
        <p><strong>Phone:</strong> +31 613950311</p>
        <br>
        <p style="color: #888; font-size: 0.85rem;" data-i18n="contactNote">For auditions, concert engagements, and project collaborations, please use the contact form or send an email directly.</p>
      </div>
      <form onsubmit="event.preventDefault(); alert('Message Sent!');">
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <input type="text" placeholder="Subject">
        <textarea rows="5" placeholder="Your Message" required></textarea>
        <button type="submit" data-i18n="sendBtn">Send Message</button>
      </form>
    </div>
  </section>

</main>

<footer>
  © Youngin Lee. All Rights Reserved. — www.younginlee.com
</footer>

<script>
const translations = {
  en: {
    navBio: "Biography", navAgenda: "Agenda & Archive", navMedia: "Media", navContact: "Contact",
    bioTitle: "Biography", downloadCv: "Download Full CV (PDF)",
    bioP1: "Korean mezzo-soprano Youngin Lee is recognized for her dark, warm timbre and deep musical intelligence. Based in Rotterdam, Netherlands, she performs across Europe in opera, oratorio, and professional ensemble projects.",
    bioP2: "Her active professional chorus engagements include the Dutch National Opera & Ballet (since 2025/26) and Groot Omroepkoor (since 2026/27) as a freelance first alto, along with participation in NKK NXT (Nederlands Kamerkoor) and her previous tenure as a Choir Academy Singer at the Wiener Staatsoper (2023/24).",
    bioP3: "Lee completed her academic formation across Korea and Germany. She holds a Bachelor of Music in Voice and a Master of Music in Musicology from Ewha Womans University, followed by a Master of Music in Opera from HfM Hanns Eisler Berlin under KS. Dr. Prof. Ewa Wolak. She was honored with the Deutschlandstipendium (2022/23), 1st Prize at the Gold International Classical Music Competition (2025), and Platinum Award at the Global Young Musicians Competition (2025).",
    eduHeader: "Education & Degrees", deg1Tag: "Bachelor Degree", deg1Name: "B.M. in Voice (Vocal Performance)",
    deg2Tag: "Master Degree 1", deg2Name: "M.M. in Opera", deg3Tag: "Master Degree 2", deg3Name: "M.M. in Musicology",
    repHeader: "Repertoire & Roles", repOperaTitle: "Opera Roles", repSacredTitle: "Oratorio & Sacred Repertoire",
    collabHeader: "Artistic Collaborators", c1: "Conductors", c2: "Stage Directors", c3: "Music Coaches", c4: "Masterclasses",
    pressHeader: "Press & Reviews", agendaTitle: "Agenda & Archive", mediaTitle: "Media",
    contactTitle: "Let's work together.", contactNote: "For auditions, concert engagements, and project collaborations, please use the contact form or send an email directly.", sendBtn: "Send Message"
  },
  de: {
    navBio: "Biografie", navAgenda: "Agenda & Archiv", navMedia: "Medien", navContact: "Kontakt",
    bioTitle: "Biografie", downloadCv: "Vollständigen CV herunterladen (PDF)",
    bioP1: "Die koreanische Mezzosopranistin Youngin Lee besticht durch ihr warmes, dunkles Timbre und ihre feine Musikalität. Von Rotterdam aus ist sie europaweit in Oper, Oratorium und professionellen Ensembles tätig.",
    bioP2: "Zu ihren aktuellen Chorengagements gehören die Dutch National Opera & Ballet (seit 2025/26) und das Groot Omroepkoor (seit 2026/27) als freischaffende 1. Altistin sowie NKK NXT (Nederlands Kamerkoor) und ihre vorherige Tätigkeit an der Wiener Staatsoper (2023/24).",
    bioP3: "Lee absolvierte ihre Ausbildung in Korea und Deutschland. Sie erwarb den Bachelor in Gesang und den Master in Musikwissenschaft an der Ewha Womans University sowie den Master in Oper an der HfM Hanns Eisler Berlin bei KS. Dr. Prof. Ewa Wolak. Sie war Stipendiatin des Deutschlandstipendiums (2022/23) und 1. Preisträgerin internationaler Wettbewerbe.",
    eduHeader: "Ausbildung & Abschlüsse", deg1Tag: "Bachelor", deg1Name: "B.M. Gesang / Gesangspädagogik",
    deg2Tag: "Master 1", deg2Name: "M.M. Oper", deg3Tag: "Master 2", deg3Name: "M.M. Musikwissenschaft",
    repHeader: "Repertoire & Rollen", repOperaTitle: "Opernrollen", repSacredTitle: "Oratorium & Sakralmusik",
    collabHeader: "Künstlerische Partner", c1: "Dirigenten", c2: "Regisseure", c3: "Korrepetitor", c4: "Meisterkurse",
    pressHeader: "Presse & Kritiken", agendaTitle: "Agenda & Archiv", mediaTitle: "Medien",
    contactTitle: "Lass uns zusammenarbeiten.", contactNote: "Für Auditions, Konzertanfragen und Projektanfragen nutzen Sie bitte das Kontaktformular.", sendBtn: "Nachricht Senden"
  },
  ko: {
    navBio: "약력", navAgenda: "공연 정보 및 아카이브", navMedia: "미디어", navContact: "연락처",
    bioTitle: "약력", downloadCv: "전체 프로필(CV) 다운로드 (PDF)",
    bioP1: "메조소프라노 이영인은 깊이 있는 음색과 뛰어난 음악적 해석력을 겸비한 성악가입니다. 현재 네덜란드 로테르담을 기반으로 오페라, 오라토리오 및 유럽 최고 수준의 전문 합창단 무대에서 활발히 활동하고 있습니다.",
    bioP2: "현재 더치 내셔널 오페라 & 발레(Dutch National Opera & Ballet, 2025/26~) 및 Groot Omroepkoor(2026/27~)의 프리랜서 1알토로 활동하고 있으며, Nederlands Kamerkoor의 NKK NXT 아티스트 및 빈 국립 오페라극장(Wiener Staatsoper, 2023/24) 합창 아카데미 단원을 역임했습니다.",
    bioP3: "이화여자대학교에서 성악 학사(B.M.) 및 음악학 석사(M.M.)를 취득한 후 베를린 한스 아이슬러 국립음대(HfM Hanns Eisler Berlin)에서 KS. Dr. Prof. Ewa Wolak 수하에서 오페라 석사(M.M.) 과정을 졸업했습니다. 독일상(Deutschlandstipendium) 장학생으로 선정되었으며, 2025년 Gold International Classical Music Competition 1위 및 Global Young Musicians Competition 플래티넘상을 수상했습니다.",
    eduHeader: "학력 과정", deg1Tag: "학사 과정", deg1Name: "성악과 학사 (B.M. Voice)",
    deg2Tag: "석사 과정 1", deg2Name: "오페라과 석사 (M.M. Opera)", deg3Tag: "석사 과정 2", deg3Name: "음악학과 석사 (M.M. Musicology)",
    repHeader: "레파토리 & 역할", repOperaTitle: "오페라 주요 역할", repSacredTitle: "오라토리오 & 종교음악",
    collabHeader: "함께한 예술가들", c1: "지휘자", c2: "연출가", c3: "음악코치 / 반주자", c4: "마스터클래스",
    pressHeader: "언론 및 언론 평", agendaTitle: "공연 정보 및 아카이브", mediaTitle: "미디어",
    contactTitle: "함께 노래해요.", contactNote: "공연 문의, 오디션 및 프로젝트 협업은 이메일이나 연동 폼을 통해 연락주시기 바랍니다.", sendBtn: "메시지 보내기"
  }
};

function setLanguage(lang) {
  document.querySelectorAll('.lang-btn').forEach(btn => btn.classList.remove('active'));
  event.target.classList.add('active');
  
  const dict = translations[lang];
  document.querySelectorAll('[data-i18n]').forEach(el => {
    const key = el.getAttribute('data-i18n');
    if (dict[key]) {
      el.textContent = dict[key];
    }
  });
}
</script>
</body>
</html>
