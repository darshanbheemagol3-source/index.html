<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Resume & Biodata — [Darshan]</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f172a; --card:#0b1220; --muted:#94a3b8; --accent:#7c3aed;
      --glass: rgba(255,255,255,0.03);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,Segoe UI,Roboto,'Helvetica Neue',Arial;background:linear-gradient(180deg,#071029 0%, #071a2b 100%);color:#e6eef8}
    .wrap{max-width:1100px;margin:32px auto;padding:24px}
    .grid{display:grid;grid-template-columns:320px 1fr;gap:20px}

    /* Sidebar */
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:20px;border-radius:14px;box-shadow:0 6px 20px rgba(2,6,23,0.6)}
    .avatar{width:96px;height:96px;border-radius:12px;overflow:hidden;background:var(--glass);display:inline-block}
    .avatar img{width:100%;height:100%;object-fit:cover;display:block}
    h1{margin:8px 0 2px;font-size:20px}
    p.role{margin:0;color:var(--muted)}
    .contact{margin-top:14px;font-size:14px;color:var(--muted)}
    .tag{display:inline-block;background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;margin:6px 6px 0 0;font-size:13px}

    /* Main */
    .tabs{display:flex;gap:6px;margin-bottom:14px}
    .tab{padding:10px 14px;border-radius:10px;background:transparent;border:1px solid transparent;cursor:pointer}
    .tab.active{background:linear-gradient(90deg,var(--accent),#4c1d95);box-shadow:0 6px 18px rgba(124,58,237,0.15)}
    .content{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:20px;border-radius:14px}
    .section{margin-bottom:18px}
    .section h3{margin:0 0 8px;font-size:16px}
    .skills{display:flex;flex-wrap:wrap}
    .skill-pill{background:rgba(255,255,255,0.03);padding:8px 10px;border-radius:8px;margin:6px 8px 6px 0;font-size:13px}
    .timeline{border-left:2px solid rgba(255,255,255,0.04);padding-left:16px}
    .timeline-item{margin-bottom:14px}
    .download-btn{display:inline-block;padding:10px 14px;border-radius:10px;background:var(--accent);color:white;text-decoration:none;margin-top:8px}

    /* Responsive */
    @media (max-width:880px){.grid{grid-template-columns:1fr;}.avatar{width:84px;height:84px}}

    /* Print */
    @media print{
      body{background:white;color:black}
      .wrap{max-width:800px}
      .tab,.download-btn{display:none}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <div class="grid">
      <aside class="card" id="sidebar">
        <div style="display:flex;gap:14px;align-items:center">
          <div class="avatar"><img id="profileImg" src="C:\Users\user\OneDrive\Desktop\assignment\profile.jpg" alt="Photo"/></div>
          <div>
            <h1 id="name">Darshan Ramakrishna Bheemagol</h1>
            <p class="role" id="title">Frontend Developer • UI/UX</p>
          </div>
        </div>

        <div class="contact" style="margin-top:16px">
          <div><strong>Email:</strong> <span id="email">darshanbheemagol@gmail.com</span></div>
          <div><strong>Phone:</strong> <span id="phone">+918660764535</span></div>
          <div><strong>Location:</strong> <span id="location">Hattaragi</span></div>
        </div>

        <div style="margin-top:12px">
          <div class="tag">Open to work</div>
          <div class="tag">Available: Immediately</div>
        </div>

        <div style="margin-top:12px;font-size:14px;color:var(--muted)">
          <strong>Education</strong>
          <div style="margin-top:6px">Computer Science Engineering — Visvesvaraya Technological University (2023 - 2027)</div>
        </div>

        <a class="download-btn" id="printBtn" href="#">Print</a>
      </aside>

      <main>
        <div class="tabs card" role="tablist">
          <button class="tab active" data-tab="resume">Resume</button>
          <button class="tab" data-tab="biodata">Biodata</button>
          <button class="tab" data-tab="portfolio">Portfolio</button>
        </div>

        <div class="content card" id="panel">
          <!-- Resume panel -->
          <section class="section" id="resume-panel">
            <h3>Professional Summary</h3>
            <p id="summary">A focused frontend developer with experience building responsive websites and web apps. Skilled in HTML, CSS, JavaScript, and modern frameworks. Passionate about creating accessible and performant user experiences.</p>

            <h3 style="margin-top:12px">Experience</h3>
            <div class="timeline">
              <div class="timeline-item">
                <strong>Frontend Developer — Acme Tech</strong>
                <div style="font-size:13px;color:var(--muted)">Jul 2027 </div>
                <div>Worked on building reusable component libraries and improved app performance by 30%.</div>
              </div>
              <div class="timeline-item">
                <strong>Web Intern Labs</strong>
                <div style="font-size:13px;color:var(--muted)">Jan 2024 — Jun 2025</div>
                <div>Built landing pages and automated testing for UI flows.</div>
              </div>
            </div>

            <h3 style="margin-top:12px">Skills</h3>
            <div class="skills" id="skills">
              <div class="skill-pill">HTML</div>
              <div class="skill-pill">CSS</div>
              <div class="skill-pill">JavaScript (ES6+)</div>
              <div class="skill-pill">jQuery</div>
              <div class="skill-pill">React (basic)</div>
              <div class="skill-pill">Git</div>
            </div>
          </section>

          <!-- Biodata panel -->
          <section class="section" id="biodata-panel" style="display:none">
            <h3>Personal Details</h3>
            <table style="width:100%;border-collapse:collapse;font-size:14px;color:var(--muted)">
              <tr><td style="padding:6px 0;width:160px">Full name</td><td id="bd-name">Darshan Ramakrishna Bheemagol</td></tr>
              <tr><td style="padding:6px 0">Father's Name</td><td id="bd-father">Ramakrishna Bheemagol</td></tr>
              <tr><td style="padding:6px 0">Mother's Name</td><td id="bd-mother">Shala Bheemagol</td></tr>
              <tr><td style="padding:6px 0">DOB</td><td id="bd-dob">15 Jan 2005</td></tr>
              <tr><td style="padding:6px 0">Gender</td><td id="bd-gender">Male</td></tr>
              <tr><td style="padding:6px 0">Marital Status</td><td id="bd-marital">Single</td></tr>
              <tr><td style="padding:6px 0">Nationality</td><td id="bd-nationality">Indian</td></tr>
              <tr><td style="padding:6px 0">Languages</td><td id="bd-langs">English, Hindi, Kannada</td></tr>
            </table>

            <h3 style="margin-top:12px">Hobbies</h3>
            <p id="hobbies">Reading, Coding, Photography</p>
          </section>

          <!-- Portfolio panel -->
          <section class="section" id="portfolio-panel" style="display:none">
            <h3>Selected Projects</h3>
            <div class="timeline">
              <div class="timeline-item">
                <strong>Project A — Sypher lock</strong>
                <div style="font-size:13px;color:var(--muted)">HTML, CSS, JS, XAMP server, PHP</div>
                <div>It is used to send documents/text privately.</div>
              </div>
              <div class="timeline-item">
                <strong>Project B — Online shoping website</strong>
                <div style="font-size:13px;color:var(--muted)">HTML, CSS, JS, PHP</div>
                <div>Online shoping app to make easy shoping for customers.</div>
              </div>
            </div>
          </section>
        </div>
      </main>
    </div>

    <footer style="text-align:center;margin-top:18px;color:var(--muted);font-size:13px">Built with plain HTML/CSS/JS — Edit this file and replace the placeholder content with your details.</footer>
  </div>

  <!-- jQuery from CDN (used as requested) -->
  <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
  <script>
    $(function(){
      // Tabs
      $('.tab').on('click', function(){
        $('.tab').removeClass('active');
        $(this).addClass('active');
        var t = $(this).data('tab');
        $('#resume-panel,#biodata-panel,#portfolio-panel').hide();
        if(t==='resume') $('#resume-panel').show();
        if(t==='biodata') $('#biodata-panel').show();
        if(t==='portfolio') $('#portfolio-panel').show();
      });

      // Download / Print
      $('#printBtn').on('click', function(e){e.preventDefault();window.print();});

      // Small helper: allow quick replace from query string ?name=...&email=...
      function qs(key){var params=new URLSearchParams(location.search);return params.get(key);}
      var qName=qs('name'); if(qName){$('#name,#bd-name,#profileName').text(qName)}
      var qEmail=qs('email'); if(qEmail)$('#email').text(qEmail);

      // Example: allow user to click avatar to upload new image (client-side only)
      var imgInput = $('<input type="file" accept="image/*" style="display:none">');
      $('body').append(imgInput);
      $('.avatar').on('click', function(){ imgInput.trigger('click'); });
      imgInput.on('change', function(e){
        var f = e.target.files && e.target.files[0]; if(!f) return;
        var reader = new FileReader(); reader.onload=function(ev){ $('#profileImg').attr('src', ev.target.result); }
        reader.readAsDataURL(f);
      });
    });
  </script>
</body>
</html>
