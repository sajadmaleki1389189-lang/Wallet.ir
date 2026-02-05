<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ولت دیجیتال - داشبورد</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <style>
    :root {
      --bg: #0d1117;
      --card: #161b22;
      --text: #c9d1d9;
      --accent: #58a6ff;
      --green: #3fb950;
      --red: #f85149;
    }
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      font-family: system-ui, -apple-system, sans-serif;
      background: var(--bg);
      color: var(--text);
      min-height: 100vh;
      padding: 16px;
    }
    .container {
      max-width: 420px;
      margin: 0 auto;
    }
    .header {
      text-align: center;
      padding: 24px 0 32px;
    }
    .header h1 {
      font-size: 2rem;
      margin-bottom: 8px;
    }
    .balance {
      font-size: 2.8rem;
      font-weight: 700;
      color: white;
    }
    .actions {
      display: flex;
      justify-content: space-around;
      margin: -20px 0 32px;
    }
    .action-btn {
      background: var(--card);
      border: 1px solid #30363d;
      border-radius: 16px;
      width: 80px; height: 80px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      color: var(--accent);
      font-size: 0.9rem;
      transition: all 0.2s;
    }
    .action-btn:hover {
      transform: translateY(-4px);
      background: #21262d;
    }
    .action-btn i { font-size: 1.8rem; margin-bottom: 4px; }
    .assets {
      background: var(--card);
      border-radius: 16px;
      padding: 16px;
      border: 1px solid #30363d;
    }
    .asset {
      display: flex;
      align-items: center;
      padding: 12px 0;
      border-bottom: 1px solid #21262d;
    }
    .asset:last-child { border-bottom: none; }
    .asset-icon {
      width: 40px; height: 40px;
      border-radius: 50%;
      background: #444;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      margin-left: 12px;
    }
    .asset-info { flex: 1; margin-right: 12px; }
    .asset-name { font-weight: 600; }
    .asset-amount { color: #8b949e; font-size: 0.9rem; }
    .asset-value {
      text-align: left;
      font-weight: 600;
    }
    .positive { color: var(--green); }
    .negative { color: var(--red); }
    .bottom-nav {
      position: fixed;
      bottom: 0; left: 0; right: 0;
      background: var(--card);
      border-top: 1px solid #30363d;
      display: flex;
      justify-content: space-around;
      padding: 12px 0;
    }
    .nav-item {
      color: #8b949e;
      font-size: 1
