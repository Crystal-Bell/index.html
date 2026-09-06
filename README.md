<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MWS Ecosystem Matrix</title>
    <style>
        body { font-family: monospace; background: #0d1117; color: #c9d1d9; padding: 20px; }
        .nav-buttons { display: flex; gap: 10px; margin-bottom: 20px; }
        button { background: #21262d; color: #58a6ff; border: 1px solid #30363d; padding: 10px 15px; cursor: pointer; font-weight: bold; }
        button:hover { background: #30363d; }
        .component-panel { display: none; border: 1px solid #30363d; padding: 20px; background: #161b22; }
        .component-panel.active { display: block; }
    </style>
</head>
<body>

    <h1>MWS Core Architecture: Ecosystem Matrix</h1>
    <p>Select a modular system component to load live operational parameters:</p>

    <div class="nav-buttons">
        <button onclick="switchComponent('prosthetics')">Avian Prosthetics</button>
        <button onclick="switchComponent('famine')">Famine & Drought</button>
        <button onclick="switchComponent('remediation')">Global Crisis Zones</button>
    </div>

    <div id="prosthetics" class="component-panel active">
        <h2>Bio-Mechanics: Avian Prosthetics</h2>
        <p>Lightweight composite matrices and structural TPU lattices for injured wildlife stabilization.</p>
    </div>

    <div id="famine" class="component-panel">
        <h2>Famine Mitigation & Drought Response</h2>
        <p>Atmospheric water harvesting and autonomous agricultural drop-delivery payloads.</p>
    </div>

    <div id="remediation" class="component-panel">
        <h2>Global Node Remediation</h2>
        <p>Decentralized manufacturing frameworks deployed across high-risk operational environments.</p>
    </div>

    <script>
        function switchComponent(componentId) {
            const panels = document.querySelectorAll('.component-panel');
            panels.forEach(panel => panel.classList.remove('active'));
            document.getElementById(componentId).classList.add('active');
        }
    </script>

</body>
</html>
# index.html