
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>DrainGuard | Smart Drain & Sanitation</title>
  
  <style>
    /* ===== GENERAL STYLES ===== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
      background: #f5f5f5;
      color: #333;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    img {
      max-width: 100%;
      height: auto;
      display: block;
    }

    /* ===== HEADER & NAVIGATION ===== */
    .nav {
      width: 100%;
      background: white;
      padding: 16px 24px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .brand {
      font-size: 24px;
      font-weight: bold;
      color: #00897b;
    }

    .brand span {
      color: #0277bd;
    }

    .nav nav {
      display: flex;
      gap: 24px;
    }

    .nav a {
      color: #555;
      font-weight: 500;
      transition: color 0.3s;
    }

    .nav a:hover {
      color: #00897b;
    }

    /* ===== MAIN LAYOUT ===== */
    main {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
    }

    /* ===== SECTION STYLES ===== */
    .section {
      padding: 40px 0;
    }

    .eyebrow {
      color: #00897b;
      font-weight: 600;
      font-size: 12px;
      letter-spacing: 1px;
      text-transform: uppercase;
      margin-bottom: 12px;
    }

    h1, h2, h3 {
      margin: 16px 0;
      color: #222;
    }

    h1 {
      font-size: 36px;
    }

    h2 {
      font-size: 28px;
    }

    h3 {
      font-size: 18px;
    }

    h1 span, h2 span {
      color: #00897b;
    }

    .lead {
      font-size: 16px;
      color: #666;
      margin: 12px 0;
    }

    .lead.small {
      font-size: 14px;
    }

    /* ===== BUTTON STYLES ===== */
    .btn {
      display: inline-block;
      padding: 12px 24px;
      border: none;
      border-radius: 6px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.3s ease;
      font-size: 14px;
      text-align: center;
    }

    .btn:disabled {
      opacity: 0.5;
      cursor: not-allowed;
    }

    .btn.primary {
      background: #00897b;
      color: white;
    }

    .btn.primary:hover:not(:disabled) {
      background: #00695c;
      box-shadow: 0 4px 8px rgba(0, 137, 123, 0.3);
    }

    .btn.secondary {
      background: #e0e0e0;
      color: #333;
      border: 1px solid #bdbdbd;
    }

    .btn.secondary:hover:not(:disabled) {
      background: #d0d0d0;
    }

    .btn.danger {
      background: #ffe6e6;
      color: #c0392b;
      border: 1px solid #f1b0b0;
    }

    .btn.danger:hover:not(:disabled) {
      background: #ffd0d0;
    }

    /* ===== HERO SECTION ===== */
    .hero {
      background: linear-gradient(135deg, #00897b 0%, #0277bd 100%);
      color: white;
      padding: 60px 40px;
      border-radius: 12px;
      text-align: center;
      margin-bottom: 40px;
    }

    .hero h1 {
      color: white;
      font-size: 40px;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #ffd54f;
    }

    .hero p {
      color: rgba(255, 255, 255, 0.9);
      font-size: 16px;
      margin-bottom: 24px;
    }

    .robot-card {
      background: rgba(255, 255, 255, 0.15);
      padding: 24px;
      border-radius: 8px;
      margin-top: 24px;
      backdrop-filter: blur(10px);
    }

    .robot-card .robot {
      font-size: 60px;
      margin-bottom: 12px;
    }

    .robot-card h3 {
      color: white;
      margin: 12px 0;
    }

    .robot-card p {
      color: rgba(255, 255, 255, 0.9);
    }

    /* ===== CARD GRID ===== */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      margin-top: 30px;
    }

    .cards article {
      background: white;
      padding: 24px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      transition: all 0.3s ease;
    }

    .cards article:hover {
      box-shadow: 0 6px 16px rgba(0, 0, 0, 0.15);
      transform: translateY(-4px);
    }

    .cards article b {
      font-size: 32px;
      display: block;
      margin-bottom: 12px;
    }

    .cards article h3 {
      margin-top: 0;
    }

    /* ===== REPORT SECTION ===== */
    .report-section {
      background: white;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }

    .report-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
      margin-top: 30px;
    }

    .panel {
      background: #fafafa;
      padding: 24px;
      border-radius: 8px;
      border: 1px solid #e0e0e0;
    }

    .panel.form {
      background: white;
      border: 2px solid #00897b;
    }

    .panel.ai-result {
      background: #f0f9f8;
      border-left: 4px solid #00897b;
    }

    /* ===== CAMERA PREVIEW ===== */
    .camera-preview {
      width: 100%;
      aspect-ratio: 1;
      background: #f5f5f5;
      border-radius: 8px;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      position: relative;
      margin-bottom: 20px;
    }

    .placeholder {
      text-align: center;
      color: #999;
    }

    .placeholder div {
      font-size: 48px;
      margin-bottom: 12px;
    }

    .placeholder strong {
      display: block;
      color: #666;
      margin: 8px 0;
    }

    #cameraVideo, #photoPreview {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    /* ===== FORM ELEMENTS ===== */
    form label {
      display: block;
      margin-bottom: 16px;
      color: #333;
      font-weight: 500;
    }

    form label input,
    form label textarea,
    form label select {
      width: 100%;
      padding: 10px;
      margin-top: 6px;
      border: 1px solid #ddd;
      border-radius: 6px;
      font-family: inherit;
      font-size: 14px;
    }

    form label input:focus,
    form label textarea:focus,
    form label select:focus {
      outline: none;
      border-color: #00897b;
      box-shadow: 0 0 0 3px rgba(0, 137, 123, 0.1);
    }

    textarea {
      resize: vertical;
      min-height: 100px;
    }

    .loc-row {
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 12px;
      align-items: flex-end;
    }

    .location-btn {
      padding: 10px 16px;
      background: #e3f2fd;
      border: 1px solid #90caf9;
      border-radius: 6px;
      cursor: pointer;
      color: #0277bd;
      font-weight: 600;
      transition: all 0.3s;
    }

    .location-btn:hover {
      background: #bbdefb;
    }

    /* ===== ACTIONS ===== */
    .actions {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
      margin: 20px 0;
    }

    .actions .btn {
      flex: 1;
      min-width: 120px;
    }

    /* ===== STATUS MESSAGES ===== */
    .status {
      padding: 12px;
      margin: 12px 0;
      border-radius: 6px;
      background: #e8f5e9;
      color: #1b5e20;
      font-size: 13px;
      border-left: 4px solid #4caf50;
    }

    .status.error {
      background: #ffebee;
      color: #b71c1c;
      border-left-color: #f44336;
    }

    .status.warning {
      background: #fff3e0;
      color: #e65100;
      border-left-color: #ff9800;
    }

    /* ===== AI SCAN STATUS ===== */
    .ai-scan-status {
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 14px;
      margin-top: 12px;
      padding: 10px;
      border-radius: 6px;
      background: #fafafa;
      border: 1px solid #e0e0e0;
    }

    .ai-scan-status.scanning {
      color: #f57c00;
      background: #fff3e0;
      border-color: #ffe0b2;
    }

    .ai-scan-status.detected {
      color: #1b5e20;
      background: #e8f5e9;
      border-color: #c8e6c9;
      font-weight: 600;
    }

    .spinner-dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: currentColor;
      animation: pulseDot 0.9s infinite ease-in-out;
      display: inline-block;
    }

    @keyframes pulseDot {
      0%, 100% {
        opacity: 0.25;
        transform: scale(0.8);
      }
      50% {
        opacity: 1;
        transform: scale(1.1);
      }
    }

    /* ===== REPORT CREATED ===== */
    .record {
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 20px;
      background: #c8e6c9;
      padding: 24px;
      border-radius: 8px;
      border-left: 4px solid #2e7d32;
      margin-top: 24px;
      align-items: center;
    }

    .badge {
      display: inline-block;
      background: #2e7d32;
      color: white;
      padding: 4px 12px;
      border-radius: 20px;
      font-size: 12px;
      font-weight: 600;
      letter-spacing: 0.5px;
      margin-bottom: 12px;
    }

    .record h3 {
      color: #1b5e20;
    }

    .record p {
      color: #2e7d32;
      font-size: 14px;
    }

    .record small {
      display: block;
      color: #558b2f;
      font-weight: 500;
      margin-bottom: 4px;
    }

    .record strong {
      color: #1b5e20;
      font-size: 18px;
      font-family: 'Courier New', monospace;
    }

    /* ===== AI RESULT ===== */
    .ai-result-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 20px;
    }

    #scanIcon {
      font-size: 28px;
    }

    .ai-result-row {
      display: grid;
      grid-template-columns: 200px 1fr;
      gap: 12px;
      padding: 12px 0;
      border-bottom: 1px solid #b2dfdb;
    }

    .ai-result-row:last-of-type {
      border-bottom: none;
    }

    .ai-result-row strong {
      color: #00695c;
    }

    .ai-confidence {
      display: grid;
      grid-template-columns: 200px 1fr;
      gap: 12px;
      padding: 12px 0;
      background: #e0f2f1;
      padding: 12px;
      border-radius: 6px;
      margin: 12px 0;
    }

    .ai-confidence strong {
      color: #00695c;
    }

    .ai-solution {
      background: white;
      padding: 16px;
      border-radius: 6px;
      margin: 16px 0;
      border-left: 4px solid #ffc107;
    }

    .ai-solution h4 {
      color: #f57f17;
      margin-bottom: 10px;
    }

    .ai-note {
      font-size: 12px;
      color: #666;
      background: white;
      padding: 12px;
      border-radius: 6px;
      margin-top: 12px;
      border: 1px dashed #ccc;
    }

    /* ===== DASHBOARD ===== */
    .dashboard {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      margin: 30px 0;
    }

    .dashboard > div {
      background: white;
      padding: 24px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    .dashboard small {
      display: block;
      color: #999;
      font-size: 12px;
      margin-bottom: 8px;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    .dashboard strong {
      font-size: 24px;
      color: #00897b;
    }

    /* ===== FOOTER ===== */
    footer {
      background: #263238;
      color: #90a4ae;
      text-align: center;
      padding: 24px;
      margin-top: 60px;
      border-top: 1px solid #37474f;
    }

    footer span {
      color: #00897b;
    }

    /* ===== RESPONSIVE ===== */
    @media (max-width: 768px) {
      .report-grid {
        grid-template-columns: 1fr;
      }

      .loc-row {
        grid-template-columns: 1fr;
      }

      .location-btn {
        width: 100%;
      }

      .nav nav {
        display: none;
      }

      .actions {
        flex-direction: column;
      }

      .actions .btn {
        width: 100%;
      }

      .record {
        grid-template-columns: 1fr;
      }

      .hero {
        padding: 40px 20px;
      }

      .hero h1 {
        font-size: 28px;
      }
    }
  </style>
</head>

<body>
  <header class="nav">
    <div class="brand">💧 Drain<span>Guard</span></div>
    <nav>
      <a href="#home">Home</a>
      <a href="#problem">Problem</a>
      <a href="#solution">Solution</a>
      <a href="#report">Report Issue</a>
      <a href="#dashboard">Dashboard</a>
    </nav>
  </header>

  <main>
    <section id="home" class="hero">
      <div>
        <p class="eyebrow">SIH 26195 • CLEAN & GREEN TECHNOLOGY</p>
        <h1>Cleaner drains.<br><span>Smarter cities.</span></h1>
        <p class="lead">A connected platform for drain inspection, citizen reporting, alerts and safer sanitation workflows.</p>
        <a class="btn primary" href="#report">Report a Drain Problem</a>
      </div>

      <div class="robot-card">
        <div class="robot">🤖</div>
        <h3>Robot-assisted inspection</h3>
        <p>Camera + sensors + dashboard for safer visual inspection.</p>
      </div>
    </section>

    <section id="problem" class="section">
      <p class="eyebrow">THE PROBLEM</p>
      <h2>Drain issues need faster visibility.</h2>

      <div class="cards">
        <article>
          <b>🌧️</b>
          <h3>Urban flooding</h3>
          <p>Blocked drains can contribute to waterlogging and delayed response.</p>
        </article>
        <article>
          <b>🦠</b>
          <h3>Health risks</h3>
          <p>Waste and stagnant water can create sanitation concerns.</p>
        </article>
        <article>
          <b>🛡️</b>
          <h3>Unsafe inspection</h3>
          <p>Remote visual checks can reduce unnecessary exposure during inspection.</p>
        </article>
      </div>
    </section>

    <section id="solution" class="section">
      <p class="eyebrow">OUR SOLUTION</p>
      <h2>One digital control layer.</h2>

      <div class="cards">
        <article>
          <h3>📷 Camera inspection</h3>
          <p>Capture visual evidence of waste, blockage or overflow risk.</p>
        </article>
        <article>
          <h3>📡 Sensor monitoring</h3>
          <p>Use water-level and flow/level trends as proposed inputs.</p>
        </article>
        <article>
          <h3>📊 Dashboard</h3>
          <p>Track reports, priorities, asset history and intervention status.</p>
        </article>
      </div>
    </section>

    <section id="report" class="section report-section">
      <p class="eyebrow">CITIZEN REPORT</p>
      <h2>Scan. Describe. Report.</h2>
      <p class="lead small">
        Open your camera, capture or upload a drain photo, let AI scan the image,
        view the detected problem and recommended solution, then create a digital issue report.
      </p>

      <div class="report-grid">
        <!-- CAMERA / PHOTO PANEL -->
        <div class="panel">
          <div class="camera-preview" id="cameraPreview">
            <div id="placeholder" class="placeholder">
              <div>📷</div>
              <strong>Camera inspection</strong>
              <span>Take a photo or upload one.</span>
            </div>

            <video id="cameraVideo" autoplay playsinline hidden></video>
            <canvas id="cameraCanvas" hidden></canvas>
            <img id="photoPreview" alt="Drain issue" hidden>
          </div>

          <div class="actions">
            <button class="btn primary" id="openCamera" type="button">Open Camera</button>
            <button class="btn secondary" id="capture" type="button" disabled>Capture Photo</button>
            <label class="btn secondary" for="photoInput">Upload Photo</label>
            <input id="photoInput" type="file" accept="image/*" hidden>
            <button class="btn danger" id="removePhoto" type="button" hidden>🗑️ Remove Photo</button>
          </div>

          <p id="cameraStatus" class="status">✓ Camera ready. Click "Open Camera" or "Upload Photo" to get started.</p>

          <!-- Live AI scan feedback appears right after a photo is captured/uploaded -->
          <p id="aiScanStatus" class="ai-scan-status" hidden></p>

          <p class="status" style="background: #e3f2fd; color: #01579b; border-left-color: #0277bd;">
            📷 Upload or capture a photo — AI will automatically scan it and suggest the problem type. You can adjust it if needed.
          </p>
        </div>

        <!-- REPORT FORM -->
        <form class="panel form" id="reportForm">
          <label>
            Your Name
            <input id="name" type="text" required placeholder="Enter your name">
          </label>

          <label>
            Problem Type
            <select id="problemType" required>
              <option value="">Select problem type</option>
              <option>Drain blockage</option>
              <option>Waste accumulation</option>
              <option>Overflow / waterlogging</option>
              <option>Damaged drain</option>
              <option>Other sanitation issue</option>
            </select>
          </label>

          <label>
            Problem Description
            <textarea id="description" required placeholder="Describe what you found..."></textarea>
          </label>

          <div class="loc-row">
            <label>
              Location
              <input id="location" type="text" required placeholder="Area / landmark / address">
            </label>
            <button type="button" class="location-btn" id="gps" title="Get your current location">📍 Use My Location</button>
          </div>

          <div class="actions">
            <button class="btn primary" type="submit">Submit Report</button>
            <button class="btn secondary" type="button" id="clear">Clear Form</button>
          </div>

          <p id="message" class="status" hidden></p>
        </form>
      </div>

      <!-- REPORT CREATED -->
      <div class="record" id="record" hidden>
        <div>
          <span class="badge">✓ REPORT CREATED</span>
          <h3 id="recordTitle"></h3>
          <p id="recordSummary"></p>
        </div>
        <div>
          <small>Issue ID</small>
          <strong id="issueId"></strong>
        </div>
      </div>
      <!-- END REPORT CREATED -->

      <!-- AI ANALYSIS AFTER REPORT SUBMISSION -->
      <div class="panel ai-result" id="aiResult" hidden>
        <div class="ai-result-header">
          <span class="badge">🤖 AI ANALYSIS COMPLETE</span>
          <span id="scanIcon">✓</span>
        </div>

        <h3>🤖 AI Scan & Recommended Solution</h3>
        <p class="lead small">AI has analyzed the submitted drain photo and provides the following recommendation.</p>

        <div class="ai-result-row">
          <strong>🔍 Problem Detected:</strong>
          <span id="detectedProblem">-</span>
        </div>

        <div class="ai-result-row">
          <strong>⚠️ Severity:</strong>
          <span id="severity">-</span>
        </div>

        <div class="ai-confidence">
          <strong>AI Confidence:</strong>
          <span id="confidence">-</span>
        </div>

        <div class="ai-solution">
          <h4>💡 Recommended Solution</h4>
          <p id="recommendedSolution"></p>
        </div>

        <p class="ai-note">
          ℹ️ <strong>Demo AI:</strong> This simple on-device image scan analyzes color/brightness patterns. In production, connect to a full computer-vision AI model for higher accuracy.
        </p>
      </div>
    </section>

    <section id="dashboard" class="section">
      <p class="eyebrow">DEMO DASHBOARD</p>
      <h2>Live monitoring concept</h2>

      <div class="dashboard">
        <div>
          <small>Robot status</small>
          <strong id="robotStatus">Ready</strong>
        </div>
        <div>
          <small>Drain condition</small>
          <strong id="drainStatus">Normal</strong>
        </div>
        <div>
          <small>Waste level</small>
          <strong id="waste">42%</strong>
        </div>
        <div>
          <small>Battery</small>
          <strong id="battery">86%</strong>
        </div>
      </div>

      <div class="actions">
        <button class="btn primary" id="demoScan" type="button">Start Demo Scan</button>
        <button class="btn secondary" id="alert" type="button">Simulate Alert</button>
      </div>
    </section>
  </main>

  <footer>
    💧 DrainGuard • Smart Waste, Drain & Sanitation Management System • SIH 26195
  </footer>

  <!-- COMPLETE INTEGRATED JAVASCRIPT -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      // ============================================================
      // CAMERA & FILE UPLOAD FUNCTIONALITY
      // ============================================================

      const openCameraBtn = document.getElementById("openCamera");
      const captureBtn = document.getElementById("capture");
      const photoInput = document.getElementById("photoInput");
      const cameraVideo = document.getElementById("cameraVideo");
      const cameraCanvas = document.getElementById("cameraCanvas");
      const photoPreview = document.getElementById("photoPreview");
      const cameraStatus = document.getElementById("cameraStatus");
      const placeholder = document.getElementById("placeholder");
      const removePhotoBtn = document.getElementById("removePhoto");

      let stream = null;

      // Open camera
      openCameraBtn.addEventListener("click", async () => {
        try {
          stream = await navigator.mediaDevices.getUserMedia({
            video: { facingMode: "environment" }
          });
          cameraVideo.srcObject = stream;
          cameraVideo.hidden = false;
          photoPreview.hidden = true;
          placeholder.hidden = true;
          captureBtn.disabled = false;
          openCameraBtn.disabled = true;
          cameraStatus.textContent = "📹 Camera is open. Click 'Capture Photo' when ready.";
          cameraStatus.style.background = "#e3f2fd";
        } catch (err) {
          cameraStatus.textContent = "❌ Camera access denied. Please check permissions.";
          cameraStatus.classList.add("error");
        }
      });

      // Capture photo from camera
      captureBtn.addEventListener("click", () => {
        const ctx = cameraCanvas.getContext("2d");
        cameraCanvas.width = cameraVideo.videoWidth;
        cameraCanvas.height = cameraVideo.videoHeight;
        ctx.drawImage(cameraVideo, 0, 0);

        // Convert canvas to image
        cameraCanvas.toBlob((blob) => {
          const url = URL.createObjectURL(blob);
          photoPreview.src = url;
          photoPreview.hidden = false;
          cameraVideo.hidden = true;
          placeholder.hidden = true;
          cameraStatus.textContent = "✓ Photo captured successfully!";

          // Stop camera
          if (stream) {
            stream.getTracks().forEach(track => track.stop());
            stream = null;
          }
          captureBtn.disabled = true;
          openCameraBtn.disabled = false;
        });
      });

      // Upload photo from file
      photoInput.addEventListener("change", (e) => {
        const file = e.target.files[0];
        if (file) {
          const reader = new FileReader();
          reader.onload = (event) => {
            photoPreview.src = event.target.result;
            photoPreview.hidden = false;
            cameraVideo.hidden = true;
            placeholder.hidden = true;
            cameraStatus.textContent = "✓ Photo uploaded successfully!";
            
            // Stop camera if open
            if (stream) {
              stream.getTracks().forEach(track => track.stop());
              stream = null;
            }
            captureBtn.disabled = true;
            openCameraBtn.disabled = false;
          };
          reader.readAsDataURL(file);
        }
      });

      // ============================================================
      // AI ANALYSIS FUNCTIONALITY
      // ============================================================

      const reportForm = document.getElementById("reportForm");
      const aiResult = document.getElementById("aiResult");
      const detectedProblem = document.getElementById("detectedProblem");
      const severity = document.getElementById("severity");
      const confidence = document.getElementById("confidence");
      const recommendedSolution = document.getElementById("recommendedSolution");
      const problemType = document.getElementById("problemType");
      const record = document.getElementById("record");
      const aiScanStatus = document.getElementById("aiScanStatus");
      const message = document.getElementById("message");

      const aiSolutions = {
        "Drain blockage": {
          severity: "High ⚠️",
          solution: "Remove accumulated waste and blockage, clean the affected drain section, and inspect water flow. If the blockage is severe, assign a maintenance team for further inspection."
        },
        "Waste accumulation": {
          severity: "Medium 🟠",
          solution: "Remove the accumulated waste safely, clean the surrounding area, and schedule regular waste collection to prevent future blockage."
        },
        "Overflow / waterlogging": {
          severity: "High ⚠️",
          solution: "Inspect the drainage path immediately, clear any obstruction, and monitor water levels. Prioritize maintenance if flooding or overflow continues."
        },
        "Damaged drain": {
          severity: "Medium 🟠",
          solution: "Inspect the damaged structure, secure the affected area if required, and arrange repair or replacement of the damaged drain section."
        },
        "Other sanitation issue": {
          severity: "Medium 🟠",
          solution: "Inspect the sanitation issue, identify the source of the problem, clean the affected area, and assign the appropriate maintenance team."
        }
      };

      // AI state
      let aiDetectedType = null;
      let aiDetectedConfidence = null;
      let userOverrode = false;

      /**
       * Lightweight AI image scan using pixel analysis
       */
      function analyzePhoto(imgEl) {
        try {
          const w = 64, h = 64;
          const c = document.createElement("canvas");
          c.width = w;
          c.height = h;
          const ctx = c.getContext("2d");
          ctx.drawImage(imgEl, 0, 0, w, h);
          const data = ctx.getImageData(0, 0, w, h).data;

          let r = 0, g = 0, b = 0, n = 0;
          let variance = 0;
          const brightnesses = [];

          for (let i = 0; i < data.length; i += 4) {
            r += data[i];
            g += data[i + 1];
            b += data[i + 2];
            brightnesses.push((data[i] + data[i + 1] + data[i + 2]) / 3);
            n++;
          }
          r /= n;
          g /= n;
          b /= n;
          const brightness = (r + g + b) / 3;

          const mean = brightness;
          for (const v of brightnesses) variance += (v - mean) * (v - mean);
          variance /= brightnesses.length;
          const stdDev = Math.sqrt(variance);

          let type, baseConfidence;

          if (b > r && b > g && brightness > 95) {
            type = "Overflow / waterlogging";
            baseConfidence = 88;
          } else if (r > g && r > b && brightness < 95) {
            type = "Drain blockage";
            baseConfidence = 85;
          } else if (g >= r && g >= b) {
            type = "Waste accumulation";
            baseConfidence = 83;
          } else if (stdDev < 18 && brightness > 120) {
            type = "Damaged drain";
            baseConfidence = 80;
          } else {
            type = "Other sanitation issue";
            baseConfidence = 76;
          }

          const spread = Math.max(Math.abs(r - g), Math.abs(g - b), Math.abs(r - b));
          const confidencePct = Math.min(97, Math.round(baseConfidence + spread / 12));

          return { type, confidence: confidencePct + "%" };
        } catch (err) {
          return null;
        }
      }

      function runScanOnCurrentPhoto() {
        if (!photoPreview.src || photoPreview.hidden) return;

        aiScanStatus.hidden = false;
        aiScanStatus.className = "ai-scan-status scanning";
        aiScanStatus.innerHTML = '<span class="spinner-dot"></span> AI is scanning the photo…';

        const doScan = () => {
          const result = analyzePhoto(photoPreview);
          if (!result) {
            aiScanStatus.className = "ai-scan-status";
            aiScanStatus.textContent = "⚠️ Could not scan automatically — please select the problem type manually.";
            return;
          }

          aiDetectedType = result.type;
          aiDetectedConfidence = result.confidence;
          userOverrode = false;

          problemType.value = aiDetectedType;

          aiScanStatus.className = "ai-scan-status detected";
          aiScanStatus.textContent = `🤖 AI detected: ${aiDetectedType} (${aiDetectedConfidence} match) — adjust if needed.`;
        };

        setTimeout(doScan, 800);
      }

      // Watch for photo changes
      const photoObserver = new MutationObserver((mutations) => {
        for (const m of mutations) {
          if ((m.attributeName === "src" || m.attributeName === "hidden") && !photoPreview.hidden && photoPreview.src) {
            removePhotoBtn.hidden = false;
            runScanOnCurrentPhoto();
          }
        }
      });
      photoObserver.observe(photoPreview, { attributes: true });

      // Remove photo
      removePhotoBtn.addEventListener("click", () => {
        photoPreview.src = "";
        photoPreview.hidden = true;
        cameraCanvas.hidden = true;
        placeholder.hidden = false;
        removePhotoBtn.hidden = true;
        photoInput.value = "";
        aiScanStatus.hidden = true;
        aiScanStatus.textContent = "";
        aiDetectedType = null;
        aiDetectedConfidence = null;
        userOverrode = false;
        aiResult.hidden = true;
        cameraStatus.textContent = "Photo removed. Take a new photo or upload another.";
      });

      // Form submission with validation
      reportForm.addEventListener("submit", (event) => {
        event.preventDefault();

        // Validate form
        const name = document.getElementById("name").value.trim();
        const location = document.getElementById("location").value.trim();
        const description = document.getElementById("description").value.trim();
        const selectedProblem = problemType.value;

        if (!name || !location || !description || !selectedProblem) {
          message.hidden = false;
          message.classList.add("error");
          message.textContent = "❌ Please fill in all fields.";
          return;
        }

        if (!photoPreview.src || photoPreview.hidden) {
          message.hidden = false;
          message.classList.add("error");
          message.textContent = "❌ Please capture or upload a photo.";
          return;
        }

        // Show success message
        message.hidden = false;
        message.classList.remove("error");
        message.textContent = "✓ Report submitted successfully! Processing AI analysis...";

        // Generate report ID
        const reportId = "DG-" + Date.now() + "-" + Math.floor(Math.random() * 1000);
        document.getElementById("recordTitle").textContent = `${selectedProblem} at ${location}`;
        document.getElementById("recordSummary").textContent = description;
        document.getElementById("issueId").textContent = reportId;
        record.hidden = false;

        // Show AI analysis after delay
        setTimeout(() => {
          let finalProblem = (aiDetectedType && !userOverrode) ? aiDetectedType : selectedProblem;

          if (!finalProblem || !aiSolutions[finalProblem]) {
            finalProblem = "Other sanitation issue";
          }

          const result = aiSolutions[finalProblem];
          const usedPhotoDetection = (finalProblem === aiDetectedType && !userOverrode);

          detectedProblem.textContent = finalProblem + (usedPhotoDetection ? " (from photo scan)" : "");
          severity.textContent = result.severity;
          confidence.textContent = usedPhotoDetection ? aiDetectedConfidence : "80%";
          recommendedSolution.textContent = result.solution;

          aiResult.hidden = false;
          aiResult.scrollIntoView({ behavior: "smooth", block: "start" });
        }, 700);
      });

      // Track if user manually changed problem type
      problemType.addEventListener("change", (event) => {
        if (event.isTrusted) {
          userOverrode = true;
        }
        aiResult.hidden = true;
      });

      // Clear form
      document.getElementById("clear").addEventListener("click", () => {
        reportForm.reset();
        aiResult.hidden = true;
        record.hidden = true;
        message.hidden = true;
        removePhotoBtn.click();
      });

      // GPS location
      document.getElementById("gps").addEventListener("click", () => {
        if (navigator.geolocation) {
          navigator.geolocation.getCurrentPosition(
            (position) => {
              const { latitude, longitude } = position.coords;
              document.getElementById("location").value = `${latitude.toFixed(4)}, ${longitude.toFixed(4)}`;
              cameraStatus.textContent = "📍 Location captured successfully!";
            },
            () => {
              message.hidden = false;
              message.classList.add("error");
              message.textContent = "❌ Location access denied.";
            }
          );
        }
      });

      // ============================================================
      // DEMO DASHBOARD
      // ============================================================

      const robotStatus = document.getElementById("robotStatus");
      const drainStatus = document.getElementById("drainStatus");
      const wasteLevel = document.getElementById("waste");
      const battery = document.getElementById("battery");

      document.getElementById("demoScan").addEventListener("click", () => {
        robotStatus.textContent = "Scanning...";
        setTimeout(() => {
          drainStatus.textContent = Math.random() > 0.5 ? "Normal" : "Blockage Detected";
          wasteLevel.textContent = Math.floor(Math.random() * 80) + 10 + "%";
          robotStatus.textContent = "Scan Complete";
        }, 2000);
      });

      document.getElementById("alert").addEventListener("click", () => {
        drainStatus.textContent = "⚠️ ALERT";
        drainStatus.style.color = "#f44336";
        wasteLevel.textContent = "95%";
        setTimeout(() => {
          drainStatus.textContent = "Normal";
          drainStatus.style.color = "inherit";
          wasteLevel.textContent = Math.floor(Math.random() * 60) + 20 + "%";
        }, 3000);
      });

      // Update battery randomly
      setInterval(() => {
        const current = parseInt(battery.textContent);
        const change = Math.floor(Math.random() * 5) - 2;
        const newValue = Math.max(5, Math.min(100, current + change));
        battery.textContent = newValue + "%";
        battery.style.color = newValue < 20 ? "#f44336" : "#00897b";
      }, 5000);
    });
  </script>
</body>
</html>
