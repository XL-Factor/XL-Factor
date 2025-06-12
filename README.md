<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>XL-Factor | GitHub README</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 0;
      background: #f5f9ff;
      color: #333;
    }
    header {
      background: #002244;
      color: white;
      padding: 2rem;
      text-align: center;
    }
    header h1 {
      font-size: 2.5rem;
      margin: 0.5rem 0;
    }
    header p {
      font-size: 1.2rem;
      color: #aad1ff;
    }
    .section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }
    .tech-icons i {
      font-size: 2rem;
      margin: 0.5rem;
      color: #0077cc;
    }
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.5rem;
      margin-top: 1rem;
    }
    .feature-card {
      background: white;
      border-radius: 12px;
      padding: 1rem;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      text-align: center;
    }
    .feature-card i {
      font-size: 2rem;
      margin-bottom: 0.5rem;
      color: #28a745;
    }
    .chart-container {
      width: 100%;
      max-width: 600px;
      margin: 2rem auto;
    }
    .button {
      display: inline-block;
      padding: 1rem 2rem;
      background: #007bff;
      color: white;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s;
    }
    .button:hover {
      background: #0056b3;
    }
    footer {
      background: #002244;
      color: white;
      padding: 2rem;
      text-align: center;
    }
    footer a {
      color: #aad1ff;
      margin: 0 0.5rem;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <h1><i class="fas fa-file-excel"></i> XL-Factor</h1>
    <p>Convert and process Excel files like never before — free and easy tools for everyone!</p>
  </header>

  <section class="section">
    <h2>🌐 Website</h2>
    <p>Visit our tools at: <a href="https://www.xl-factor.com" class="button" target="_blank">www.xl-factor.com</a></p>
  </section>

  <section class="section">
    <h2>🚀 Supported Technologies</h2>
    <div class="tech-icons">
      <i class="fab fa-html5"></i>
      <i class="fab fa-css3-alt"></i>
      <i class="fab fa-js"></i>
      <i class="fas fa-file-excel"></i>
      <i class="fas fa-file-csv"></i>
      <i class="fas fa-file-pdf"></i>
      <i class="fas fa-database"></i>
    </div>
  </section>

  <section class="section">
    <h2>🧰 Tools Offered</h2>
    <div class="features">
      <div class="feature-card"><i class="fas fa-file-import"></i><p>Excel to CSV, PDF, JSON</p></div>
      <div class="feature-card"><i class="fas fa-file-export"></i><p>CSV, PDF, JSON to Excel</p></div>
      <div class="feature-card"><i class="fas fa-layer-group"></i><p>Merge Excel Files</p></div>
      <div class="feature-card"><i class="fas fa-table"></i><p>Merge or Split Sheets</p></div>
      <div class="feature-card"><i class="fas fa-search"></i><p>VLOOKUP & Advanced Lookup</p></div>
      <div class="feature-card"><i class="fas fa-image"></i><p>Image VLOOKUP</p></div>
    </div>
  </section>

  <section class="section">
    <h2>📊 Popular Usage Stats</h2>
    <div class="chart-container">
      <canvas id="usageChart"></canvas>
    </div>
  </section>

  <footer>
    <p>Made with ❤️ by Bharat S Kharat</p>
    <p>
      <a href="https://www.github.com/xl-factor" target="_blank"><i class="fab fa-github"></i> GitHub</a>
      <a href="mailto:info@xl-factor.com"><i class="fas fa-envelope"></i> Contact</a>
    </p>
    <p>&copy; 2025 XL-Factor. MIT License.</p>
  </footer>

  <script>
    const ctx = document.getElementById('usageChart').getContext('2d');
    new Chart(ctx, {
      type: 'pie',
      data: {
        labels: ['Excel to PDF', 'Merge Sheets', 'Image VLOOKUP', 'Excel to JSON', 'Split Sheets'],
        datasets: [{
          label: 'Tool Usage',
          data: [30, 25, 20, 15, 10],
          backgroundColor: ['#007bff', '#28a745', '#ffc107', '#17a2b8', '#dc3545']
        }]
      }
    });
  </script>
</body>
</html>
