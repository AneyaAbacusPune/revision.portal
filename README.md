<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aneya Abacus | Professional Assessment Portal</title>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        /* Modern Design System */
        :root {
            --primary: #165430;
            --secondary: #f36621;
            --bg: #f4f7f6;
            --text: #2d3436;
        }

        body { 
            background-color: var(--bg); 
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; 
            margin: 0; display: flex; justify-content: center; align-items: center; 
            min-height: 100vh; color: var(--text);
        }

        .card { 
            background: #ffffff; padding: 40px; border-radius: 20px; 
            box-shadow: 0 20px 40px rgba(0,0,0,0.08); text-align: center; 
            width: 90%; max-width: 420px;
        }

        h2 { color: var(--primary); font-size: 24px; margin-bottom: 30px; }
        
        input, select { 
            width: 100%; padding: 15px; margin-bottom: 20px; border: 1.5px solid #e1e8ed; 
            border-radius: 12px; font-size: 16px; transition: 0.3s;
        }
        input:focus { outline: none; border-color: var(--secondary); }

        button { 
            border: none; padding: 15px 25px; border-radius: 12px; font-size: 16px; 
            font-weight: 600; cursor: pointer; transition: all 0.3s; color: white;
        }
        
        /* Layout & Exam Section */
        #examSection { 
            display: none; background: white; padding: 30px; border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1); width: 95%; max-width: 900px;
        }

        .exam-grid { display: grid; grid-template-columns: 2fr 1fr; gap: 30px; }
        
        .header-bar { 
            display: flex; justify-content: space-between; align-items: center; 
            background: #f8f9fa; padding: 15px 20px; border-radius: 12px; margin-bottom: 20px; 
        }

        .math-display { font-size: 42px; font-weight: 700; margin: 40px 0; letter-spacing: 5px; }

        .btn-group { display: flex; gap: 10px; margin-top: 20px; }
        .btn-primary { background: var(--secondary); flex: 1; }
        .btn-secondary { background: var(--primary); flex: 1; }

        /* Palette styling */
        .palette { display: grid; grid-template-columns: repeat(5, 1fr); gap: 8px; }
        .p-btn { 
            padding: 10px; border-radius: 8px; border: 1px solid #eee; 
            background: #f8f9fa; cursor: pointer; font-weight: bold; 
        }
        .p-btn.active { background: var(--primary); color: white; }
        .p-btn.done { background: #d4edda; color: var(--primary); }

        @media (max-width: 768px) { .exam-grid { grid-template-columns: 1fr; } }
    </style>
</head>
<body>
    <div id="loginSection" class="card">
        <h2>Aneya Abacus Portal</h2>
        <input type="number" id="mobileInput" placeholder="Mobile Number">
        <input type="password" id="passwordInput" placeholder="Password">
        <div class="btn-group">
            <button class="btn-secondary" onclick="login('dashboard')">Dashboard</button>
            <button class="btn-primary" onclick="login('exam')">Revision</button>
        </div>
    </div>
    
    </body>
</html>
