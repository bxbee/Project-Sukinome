<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Google Vision API Overview</title>
  <style>
    :root {
      --bg: #0f172a;
      --card: #111827;
      --text: #e5e7eb;
      --muted: #9ca3af;
      --accent: #34d399;
      --accent2: #60a5fa;
      --border: #1f2937;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, "Helvetica Neue", Arial, "Noto Sans", sans-serif;
      background: radial-gradient(1200px 600px at 20% 0%, #0b1324 20%, var(--bg)), var(--bg);
      color: var(--text);
      line-height: 1.5;
    }

    .container {
      max-width: 900px;
      margin: 40px auto;
      padding: 0 20px;
    }

    .card {
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)),
                  var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 28px;
      box-shadow:
        0 10px 30px rgba(0,0,0,0.35),
        inset 0 1px 0 rgba(255,255,255,0.04);
    }

    .title {
      display: flex;
      align-items: center;
      gap: 12px;
      margin: 0 0 8px;
      font-size: 28px;
      letter-spacing: 0.3px;
    }

    .badge {
      display: inline-block;
      font-size: 12px;
      color: #0b1324;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      padding: 4px 10px;
      border-radius: 999px;
      font-weight: 600;
    }

    .subtitle {
      margin: 10px 0 24px;
      color: var(--muted);
      font-size: 15px;
    }

    h2 {
      margin: 22px 0 10px;
      font-size: 20px;
      letter-spacing: 0.2px;
    }

    .list {
      margin: 0;
      padding: 0;
      list-style: none;
      display: grid;
      gap: 10px;
    }

    .list li {
      position: relative;
      padding: 10px 12px 10px 36px;
      border: 1px solid var(--border);
      border-radius: 12px;
      background: rgba(255,255,255,0.02);
    }

    .list li::before {
      content: "✔";
      position: absolute;
      left: 12px;
      top: 50%;
      transform: translateY(-50%);
      color: var(--accent);
      font-weight: 700;
    }

    .pill {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      border: 1px dashed var(--border);
      border-radius: 999px;
      padding: 8px 12px;
      color: var(--muted);
      font-size: 13px;
      margin: 8px 8px 0 0;
      background: rgba(96, 165, 250, 0.06);
    }

    .footer {
      margin-top: 24px;
      font-size: 12px;
      color: var(--muted);
    }

    @media (max-width: 520px) {
      .title { font-size: 24px; }
      .card { padding: 22px; }
    }
  </style>
</head>
<body>
  <div class="container">
    <section class="card" aria-labelledby="vision-title">
      <h1 id="vision-title" class="title">
        Google Vision API
        <span class="badge" aria-label="Category">Image AI</span>
      </h1>
      <p class="subtitle">
        Google Vision API is a powerful tool for analyzing and understanding images. It supports face detection, object detection, and image labeling.
      </p>

      <h2>Key Features</h2>
      <ul class="list">
        <li><strong>Automatic image detection:</strong> Identifies and processes images automatically.</li>
        <li><strong>Object detection:</strong> Recognizes and classifies objects in an image.</li>
        <li><strong>Face detection:</strong> Detects human faces for tagging and analytics.</li>
        <li><strong>Image identification:</strong> Labels and categorizes images for easier search and organization.</li>
      </ul>

      <h2>Deploy and Integrate</h2>
      <div>
        <span class="pill">Vertex AI (Google Cloud)</span>
        <span class="pill">AWS SageMaker (integration via outputs)</span>
      </div>

      <div class="footer">
        Note: Features and pricing may vary depending on your usage and platform setup.
      </div>
    </section>
  </div>
</body>
</html>
