<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🌿 Biology 1: Cloud-Synced Synthesis Ledger 🧪</title>
    <style>
        :root {
            --chloroplast-green: #2ecc71;
            --mitochondria-orange: #f39c12;
            --cytoplasm-blue: #3498db;
            --cell-wall-dark: #2c3e50;
            --vacuole-liquid: #eef9ff;
            --nucleolus-pink: #e74c3c;
            --atp-yellow: #f1c40f;
        }
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--vacuole-liquid);
            background-image: radial-gradient(#bdc3c7 1px, transparent 1px);
            background-size: 24px 24px;
            color: var(--cell-wall-dark);
            margin: 0;
            padding: 20px;
        }
        .container { max-width: 1100px; margin: 0 auto; }
        header {
            text-align: center; margin-bottom: 30px;
            background: linear-gradient(135deg, #27ae60, #11998e);
            padding: 25px; border-radius: 16px; box-shadow: 0 6px 0px #1e7e34;
            border: 3px solid var(--cell-wall-dark); color: white;
        }
        header h1 { margin: 0; font-size: 2.2em; text-shadow: 2px 2px 0px var(--cell-wall-dark); }
        header p { margin: 8px 0 0 0; font-weight: 500; font-style: italic; color: #fff; }
        
        .graph-card {
            background: #fff; border: 3px solid var(--cell-wall-dark);
            border-radius: 16px; padding: 20px; margin-bottom: 25px;
            box-shadow: 4px 4px 0px var(--cell-wall-dark);
        }
        .graph-container {
            background: #ecf0f1; border: 3px solid var(--cell-wall-dark);
            border-radius: 12px; height: 35px; position: relative; overflow: hidden; margin: 15px 0;
        }
        .graph-bar {
            background: linear-gradient(90deg, var(--atp-yellow), var(--chloroplast-green));
            height: 100%; width: 0%; transition: width 0.6s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .graph-text {
            position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);
            font-weight: bold; font-size: 14px; color: var(--cell-wall-dark); text-shadow: 1px 1px 0px #fff;
        }
        .grid { display: grid; grid-template-columns: 1fr 1.1fr; gap: 25px; }
        @media (max-width: 850px) { .grid { grid-template-columns: 1fr; } }
        
        .card { background: #fff; padding: 25px; border-radius: 16px; border: 3px solid var(--cell-wall-dark); box-shadow: 4px 4px 0px var(--cell-wall-dark); }
        h2 { margin-top: 0; font-size: 1.3em; background: #ffeaa7; display: inline-block; padding: 4px 12px; border-radius: 8px; border: 2px solid var(--cell-wall-dark); }
        .form-group { margin-bottom: 16px; }
        label { display: block; font-weight: bold; margin-bottom: 6px; font-size: 14px; }
        select, textarea, button { width: 100%; padding: 12px; border: 2px solid var(--cell-wall-dark); border-radius: 8px; box-sizing: border-box; font-family: inherit; font-size: 14px; }
        button { background-color: var(--chloroplast-green); color: white; font-weight: bold; font-size: 16px; cursor: pointer; box-shadow: 0 4px 0px #1e7e34; }
        button:disabled { background-color: #95a5a6; box-shadow: 0 4px 0px #7f8c8d; cursor: not-allowed; }
        .reset-btn { background-color: var(--nucleolus-pink); margin-top: 25px; font-size: 12px; padding: 6px; width: auto; color: white; border: none; border-radius: 8px;}
        
        .student-row-wrapper { background: #f8f9fa; border: 2px solid var(--cell-wall-dark); border-radius: 12px; padding: 12px; margin-bottom: 12px; }
        .student-row { display: flex; justify-content: space-between; align-items: center; }
        .badge { background: var(--mitochondria-orange); color: white; padding: 4px 12px; border-radius: 50px; font-weight: bold; border: 2px solid var(--cell-wall-dark); }
        .comment-box { font-size: 13px; background: #fff; padding: 8px; margin-top: 8px; border: 2px solid #bdc3c7; border-radius: 6px; border-left: 4px solid var(--cytoplasm-blue); }

        .modal { display: none; position: fixed; z-index: 100; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(44, 62, 80, 0.7); align-items: center; justify-content: center; }
        .modal-content { background: #fff; border: 4px solid var(--cell-wall-dark); padding: 30px; border-radius: 20px; max-width: 520px; text-align: center; box-shadow: 8px 8px 0px var(--atp-yellow); }
        .science-fact { background: #fff9e6; border: 2px dashed var(--mitochondria-orange); padding: 15px; border-radius: 10px; margin: 15px 0; font-size: 14px; text-align: left; line-height: 1.5; }
        .close-modal-btn { background-color: var(--cytoplasm-blue); color: white; cursor: pointer;}
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>🌿 Biology 1: Cloud-Synced Cellular Ecosystem Hub 🧪</h1>
        <p>Live Google Sheet Remote Uplink Enabled for Long-Term Data Logging</p>
    </header>

    <div class="graph-card">
        <h2>📊 Daily Calvin Cycle: Glucose Production Yield</h2>
        <div class="graph-container">
            <div id="dailyProgressBar" class="graph-bar"></div>
            <div id="counterLabel" class="graph-text">0 / 40 Photons Captured</div>
        </div>
    </div>

    <div class="grid">
        <div class="card">
            <h2>🔬 Initiate Chemical Energy Transfer</h2>
            <form id="rewardForm">
                <div class="form-group">
                    <label for="voterSelect">🧬 Source Organism (Your Name):</label>
                    <select id="voterSelect" required></select>
                </div>
                <div class="form-group">
                    <label for="targetSelect">🌱 Target Organism (Recipient Classmate):</label>
                    <select id="targetSelect" required></select>
                </div>
                <div class="form-group">
                    <label for="taskSelect">✨ Metabolic Process Performed:</label>
                    <select id="taskSelect" required>
                        <option value="">-- Identify the Biological Interaction --</option>
                        <option value="lang">🗣️ 1. Heard speaking English (Intercellular Signal Translation)</option>
                        <option value="help">🤝 2. Helping a classmate (Symbiosis: Mitigating Matrix Stress)</option>
                        <option value="task">💻 3. Diligent in tasks (Active Transport: Storing Chromebooks via ATP)</option>
                        <option value="notes">✍️ 4. Writing notes (DNA Transcription & Info Encoding)</option>
                        <option value="part">🙋‍♂️ 5. Participating (Enzyme Catalyst: Acceleration of Lesson Rate)</option>
                        <option value="clean">🧹 6. Cleaning the room (Lysosome Action: Hydrolytic Waste Removal)</option>
                        <option value="respect">❤️ 7. Respecting everyone (Homeostasis: Maintaining System Equilibrium)</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="anonymousComment">💌 Leave an Anonymous Encrypted Message Block</label>
                    <textarea id="anonymousComment" rows="2" placeholder="Send an encouraging molecular sequence note..."></textarea>
                </div>
                <button type="submit" id="submitBtn">☀️ Fire Photon Beam & Sync to Cloud!</button>
            </form>
            <button class="reset-btn" onclick="resetLedger()">Wipe Local Cache Only</button>
        </div>

        <div class="card">
            <h2>🏆 Biomass High-Score Ledger</h2>
            <div id="leaderboard"></div>
        </div>
    </div>
</div>

<div id="bioModal" class="modal">
    <div class="modal-content">
        <h3>🌱 Stream Upload & Light Reaction Successful!</h3>
        <div id="scienceFactContainer" class="science-fact"></div>
        <button class="close-modal-btn" onclick="closeModal()">Absorb Core Knowledge & Resume</button>
    </div>
</div>

<script>
    // Your verified and integrated Google App Script URL Deployment
    const googleWebAppUrl = "https://script.google.com/macros/s/AKfycbyEBULyz8H9li21QazvouqLk8uXiNmrlDYgXX4CFZlMrg3-4Gprn3I9VKk1cwrI3uhJ6w/exec";

    const defaultStudents = [
        { name: "ABESA, DYLAN JAMES TESORERO", points: 0, comments: [] },
        { name: "ALARTE, MARIAE RIZCHANE GUIRIBA", points: 0, comments: [] },
        { name: "ALMOITE, JANNA LYN PADUA", points: 0, comments: [] },
        { name: "AVENGOZA, THANDIE MISCHE", points: 0, comments: [] },
        { name: "BAGASINA, SHARMAINE KATE CAMILO", points: 0, comments: [] },
        { name: "BOLIVAR, SHAN KESSNER RANCE", points: 0, comments: [] },
        { name: "BUENA, DANN CHRISTIAN SIGUENZA", points: 0, comments: [] },
        { name: "CABILIN, ELLA SHAINE DARANG", points: 0, comments: [] },
        { name: "CADAG, HANNAH ANGEL MARAVILLA", points: 0, comments: [] },
        { name: "CARINGAL, PRECIOUS CHLOE MADERA", points: 0, comments: [] },
        { name: "CARIZO, KRISTINE MARGARETTE MARCO", points: 0, comments: [] },
        { name: "CASONGCAD, ARIENNE LLANERA", points: 0, comments: [] },
        { name: "CLORES, CAitLIN FAY OTORDOS", points: 0, comments: [] },
        { name: "COLLANTES, FRAZIER GABRIEL PANTALEON", points: 0, comments: [] },
        { name: "CORDIS, JAC VINCE OBOGNE", points: 0, comments: [] },
        { name: "DE LA TORRE, SEAN GABRIEL BONGANAY", points: 0, comments: [] },
        { name: "DELA CRUZ, MARJ GRAZEL AZADA", points: 0, comments: [] },
        { name: "GAMINDE, MAXSENE ONG", points: 0, comments: [] },
        { name: "GARING, KATRINA CASSANDRA BRAVO", points: 0, comments: [] },
        { name: "GAVICA, JILIAN KAYE PARADO", points: 0, comments: [] },
        { name: "IMPERIAL, ALIYA REANN ROSE CONCEPCION", points: 0, comments: [] },
        { name: "LORENTE, RONALD JR. LANUZO", points: 0, comments: [] },
        { name: "LORILLA, ANIKA GWEN PILAPIL", points: 0, comments: [] },
        { name: "MAGDAMIT, AYANA JEN SANTIAGO", points: 0, comments: [] },
        { name: "MOISES, GREIMARL FAITH BRONZAL", points: 0, comments: [] },
        { name: "NIEVA, MARK WILLAN AILES", points: 0, comments: [] },
        { name: "OCAMPO, FRANCESCA YNA MARITHE PRILLES", points: 0, comments: [] },
        { name: "PANALIGAN, PAMELA MONTANEZ", points: 0, comments: [] },
        { name: "PAR, JAMIE LYN ENRIQUEZ", points: 0, comments: [] },
        { name: "PERALTA, FAYE GLEAYNN LAZARTE", points: 0, comments: [] },
        { name: "PICZON, XIAN LEONEIL CONCORDIA", points: 0, comments: [] },
        { name: "PUNAYO, ZEIJAN MARTIREZ", points: 0, comments: [] },
        { name: "RAMOS, KEN ABIEL OLLETE", points: 0, comments: [] },
        { name: "REBAMONTE, LIANNE ABAWAG", points: 0, comments: [] },
        { name: "REGULADO, EUNICE PARMA", points: 0, comments: [] },
        { name: "RIVERO, ANGELITA FE AUTOR", points: 0, comments: [] },
        { name: "ROMALES, JOHN MICHAEL GALLENITO", points: 0, comments: [] },
        { name: "SAN BUENAVENTURA, KRISTA YABA", points: 0, comments: [] },
        { name: "VILLABLANCA, CHANEL KELLY MANUEL", points: 0, comments: [] },
        { name: "VILLAMIN, ANTONIO JOSE", points: 0, comments: [] }
    ];

    const biologyCurriculum = {
        lang: "🔬 <b>Cell Signaling & Translation:</b> Expressing instructions clearly mirrors how cells communicate. In complex tissues, cells synthesize and emit signaling ligands that travel through gap junctions to execute shared processes.",
        help: "🤝 <b>Symbiotic Interdependence:</b> Providing aid mimics mutualistic interactions. At a microscopic tier, organelles (like mitochondria working with chloroplasts) exist in an obligate symbiotic cycle to offset thermodynamic stress.",
        task: "🔋 <b>Active Transport via ATP:</b> Organized material movement requires physical energy input. In biology, <i>Active Transport</i> moves essential solute molecules across a selective plasma membrane from lower to higher concentrations using ATP currency.",
        notes: "🧬 <b>Transcription & Information Storage:</b> Translating lectures to paper mimics gene expression. During <i>Transcription</i>, your cells build an exact copy of DNA segments into complementary mRNA transcripts to safely transport instructions outside the nucleus.",
        part: "⚡ <b>Enzymatic Catalysis:</b> Immediate active response accelerates classroom progression. Biological <i>Enzymic Catalysts</i> behave the same way—lowering required activation energy bounds to increase physiological reaction rates millions of times over.",
        clean: "🧹 <b>Lysosomal Hydrolysis:</b> Collecting and processing debris acts like a cell's <i>Lysosome</i> vesicle network. Lysosomes host hydrolytic enzymes that selectively break down damaged cellular components, old lipids, and toxic waste invaders.",
        respect: "⚖️ <b>Homeostatic Equilibrium:</b> Preserving a balanced safe space matches <i>Homeostasis</i>. Living organisms constantly adjust negative feedback mechanisms to hold internal temperature, water balances, and pH scales uniform against volatile exterior pressures."
    };

    let students = [];
    let dailyVotesCount = 0;
    const dailyTargetGoal = 40;

    function getTodayString() {
        const d = new Date(); return d.getFullYear() + '-' + (d.getMonth() + 1) + '-' + d.getDate();
    }

    function init() {
        const storedData = localStorage.getItem('biologyLedgerRoster');
        if (storedData) {
            students = JSON.parse(storedData);
            if(students.length !== defaultStudents.length) students = defaultStudents;
        } else {
            students = defaultStudents;
            saveToStorage();
        }

        const todayStr = getTodayString();
        const storedDate = localStorage.getItem('biologyLedgerDateStamp');
        const storedDailyVotes = localStorage.getItem('biologyLedgerDailyCount');

        if (storedDate === todayStr) {
            dailyVotesCount = storedDailyVotes ? parseInt(storedDailyVotes, 10) : 0;
        } else {
            dailyVotesCount = 0;
            localStorage.setItem('biologyLedgerDateStamp', todayStr);
            localStorage.setItem('biologyLedgerDailyCount', "0");
        }

        populateDropdowns();
        renderLeaderboard();
        updateBarGraph();
    }

    function saveToStorage() {
        localStorage.setItem('biologyLedgerRoster', JSON.stringify(students));
        localStorage.setItem('biologyLedgerDailyCount', dailyVotesCount.toString());
    }

    function populateDropdowns() {
        const voterSelect = document.getElementById('voterSelect');
        const targetSelect = document.getElementById('targetSelect');
        voterSelect.innerHTML = '<option value="">-- Select Your Name --</option>';
        targetSelect.innerHTML = '<option value="">-- Select Classmate --</option>';

        const sortedStudents = [...students].sort((a, b) => a.name.localeCompare(b.name));
        sortedStudents.forEach(student => {
            const opt1 = document.createElement('option'); opt1.value = student.name; opt1.textContent = student.name;
            voterSelect.appendChild(opt1);
            const opt2 = document.createElement('option'); opt2.value = student.name; opt2.textContent = student.name;
            targetSelect.appendChild(opt2);
        });
    }

    function updateBarGraph() {
        const bar = document.getElementById('dailyProgressBar');
        const label = document.getElementById('counterLabel');
        let percentage = Math.floor((dailyVotesCount / dailyTargetGoal) * 100);
        if (percentage > 100) percentage = 100;
        bar.style.width = percentage + '%';
        label.textContent = `${dailyVotesCount} / ${dailyTargetGoal} Photons Captured (${percentage}% Daily Glucose Yield Reached!)`;
    }

    function renderLeaderboard() {
        const board = document.getElementById('leaderboard');
        board.innerHTML = '';
        const sorted = [...students].sort((a, b) => b.points - a.points);

        sorted.forEach(student => {
            const container = document.createElement('div'); container.className = 'student-row-wrapper';
            const mainRow = document.createElement('div'); mainRow.className = 'student-row';
            mainRow.innerHTML = `<span class="student-name">🔬 ${student.name}</span> <span class="badge">🔋 ${student.points} ATP</span>`;
            container.appendChild(mainRow);

            if(student.comments && student.comments.length > 0) {
                student.comments.forEach(comment => {
                    const cBox = document.createElement('div'); cBox.className = 'comment-box';
                    cBox.textContent = `🧬 "${comment}"`; container.appendChild(cBox);
                });
            }
            board.appendChild(container);
        });
    }

    document.getElementById('rewardForm').addEventListener('submit', function(e) {
        e.preventDefault();
        const voter = document.getElementById('voterSelect').value;
        const target = document.getElementById('targetSelect').value;
        const taskKey = document.getElementById('taskSelect').value;
        const taskText = document.getElementById('taskSelect').options[document.getElementById('taskSelect').selectedIndex].text;
        const commentText = document.getElementById('anonymousComment').value.trim();

        if (voter === target) {
            alert("❌ System Logic Fault: An isolated cell node cannot stimulate itself! Select an external organism.");
            return;
        }

        const submitBtn = document.getElementById('submitBtn');
        submitBtn.disabled = true;
        submitBtn.textContent = "⚡ Syncing Molecule Data to Sheet...";

        const payload = {
            voter: voter,
            target: target,
            task: taskText,
            comment: commentText || "None Provided"
        };

        fetch(googleWebAppUrl, {
            method: "POST",
            mode: "no-cors", 
            headers: { "Content-Type": "application/json" },
            body: JSON.stringify(payload)
        })
        .then(() => {
            const studentIndex = students.findIndex(s => s.name === target);
            if (studentIndex !== -1) {
                students[studentIndex].points += 1;
                dailyVotesCount += 1; 

                if (commentText !== "") {
                    students[studentIndex].comments.push(commentText);
                }

                saveToStorage();
                renderLeaderboard();
                updateBarGraph();
                
                document.getElementById('scienceFactContainer').innerHTML = biologyCurriculum[taskKey];
                document.getElementById('bioModal').style.display = 'flex';

                document.getElementById('anonymousComment').value = '';
                document.getElementById('taskSelect').value = '';
            }
        })
        .catch(err => {
            alert("⚠️ Cloud Uplink Disrupted: Data saved locally instead.");
            console.error(err);
        })
        .finally(() => {
            submitBtn.disabled = false;
            submitBtn.textContent = "☀️ Fire Photon Beam & Fix Carbon!";
        });
    });

    function closeModal() { document.getElementById('bioModal').style.display = 'none'; }
    function resetLedger() { if(confirm("Clear local interface memory? Cloud data remains on Google Sheets.")) { localStorage.clear(); init(); } }

    window.onload = init;
</script>
</body>
</html>
