<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mohammad Muaz Mohiuddin - Coursework Portfolio</title>
    <style>
        :root {
            --primary-color: #0f172a;
            --accent-color: #0284c7;
            --bg-color: #f8fafc;
            --card-bg: #ffffff;
            --text-main: #334155;
            --text-dark: #0f172a;
            --border-color: #e2e8f0;
        }

        body {
            font-family: 'Segoe UI', system-ui, sans-serif;
            line-height: 1.6;
            color: var(--text-main);
            background-color: var(--bg-color);
            margin: 0;
            padding: 0;
        }

        .profile-banner {
            background-color: var(--primary-color);
            color: #ffffff;
            padding: 50px 20px;
            text-align: center;
            border-bottom: 4px solid var(--accent-color);
        }

        .banner-content {
            max-width: 900px;
            margin: 0 auto;
        }

        .banner-content h1 {
            margin: 0 0 10px 0;
            font-size: 2.4rem;
            font-weight: 700;
        }

        .banner-content .programme {
            font-size: 1.2rem;
            color: #93c5fd;
            margin: 5px 0 20px 0;
            font-weight: 500;
        }

        .academic-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            background: rgba(255, 255, 255, 0.08);
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
            font-size: 0.95rem;
            text-align: left;
        }

        .grid-item strong {
            color: #e2e8f0;
            display: block;
            font-size: 0.8rem;
            text-transform: uppercase;
            margin-bottom: 2px;
        }

        .layout-container {
            max-width: 1000px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .portfolio-intro {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 25px;
            margin-bottom: 35px;
        }

        .portfolio-intro h2 {
            margin-top: 0;
            color: var(--text-dark);
        }

        .manager-panel {
            background: #f1f5f9;
            border: 2px dashed #cbd5e1;
            padding: 25px;
            border-radius: 8px;
            margin-bottom: 40px;
        }

        .manager-panel h3 {
            margin-top: 0;
            color: var(--text-dark);
        }

        label {
            display: block;
            margin-top: 12px;
            font-weight: 600;
            font-size: 0.9rem;
            color: var(--text-dark);
        }

        select, input[type="text"], textarea {
            width: 100%;
            padding: 12px;
            margin-top: 6px;
            box-sizing: border-box;
            border: 1px solid #cbd5e1;
            border-radius: 6px;
            background: #ffffff;
        }

        .btn-submit {
            background-color: var(--accent-color);
            color: white;
            padding: 12px 24px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            margin-top: 15px;
        }

        .btn-submit:hover { background-color: #0369a1; }

        .chapter-list {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        .chapter-card {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 30px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }

        .chapter-card h2 {
            margin-top: 0;
            color: var(--text-dark);
            font-size: 1.4rem;
            border-bottom: 2px solid #f1f5f9;
            padding-bottom: 12px;
        }

        .chapter-content {
            white-space: pre-wrap;
            color: var(--text-main);
            font-size: 1rem;
        }

        .btn-clear {
            background: #ef4444;
            color: white;
            border: none;
            padding: 6px 12px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 0.85rem;
            margin-top: 15px;
        }

        @media print { .manager-panel, .btn-clear { display: none; } }
    </style>
</head>
<body>

    <header class="profile-banner">
        <div class="banner-content">
            <h1>Mohammad Muaz Mohiuddin</h1>
            <div class="programme">Bachelor of Electronics Engineering with Honours (Mechatronics)</div>
            
            <div class="academic-grid">
                <div class="grid-item"><strong>Student ID</strong>B122510871</div>
                <div class="grid-item"><strong>Course Code</strong>BERR1233</div>
                <div class="grid-item"><strong>University</strong>Universiti Teknikal Malaysia Melaka</div>
                <div class="grid-item"><strong>Lecturer</strong>Dr. Nurul Fajar</div>
                <div class="grid-item"><strong>Year / Semester</strong>Year 1 / Semester 2</div>
                <div class="grid-item"><strong>Academic Session</strong>2025/2026</div>
            </div>
        </div>
    </header>

    <div class="layout-container">
        
        <div class="portfolio-intro">
            <h2>Coursework Documentation Hub</h2>
            <p>Welcome to my digital learning portfolio. This space serves as an academic log showcasing concepts, structures, implementation techniques, and theoretical foundations explored throughout the course duration.</p>
        </div>

        <div class="manager-panel">
            <h3>Update Chapter Information</h3>
            <p style="margin: 0 0 10px 0; font-size: 0.85rem; color: #64748b;">Select a module to customize or add content updates.</p>
            
            <label for="chapter-select">Target Module Section:</label>
            <select id="chapter-select">
                <option value="0">Chapter 1: Introduction to Data Structures</option>
                <option value="1">Chapter 2: Fundamentals of C++</option>
                <option value="2">Chapter 3: Arrays</option>
                <option value="3">Chapter 4: Abstract Data Types</option>
                <option value="4">Chapter 5: Stack</option>
                <option value="5">Chapter 6: Queue</option>
                <option value="7">Chapter 7: Sorting Algorithms</option>
                <option value="8">Chapter 8: Searching Algorithms</option>
                <option value="9">Chapter 9: Linked List</option>
                <option value="10">Chapter 10: Tree</option>
            </select>

            <label for="chapter-body">Slide Notes / Compilation Content:</label>
            <textarea id="chapter-body" rows="6" placeholder="Paste your slide contents or sample notes here..."></textarea>
            
            <button class="btn-submit" onclick="saveChapterData()">Update Portfolio Content</button>
        </div>

        <div class="chapter-list" id="portfolio-container">
            </div>

    </div>

    <script>
        const systemChapters = [
            { id: 0, heading: "Chapter 1: Introduction to Data Structures", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 1, heading: "Chapter 2: Fundamentals of C++", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 2, heading: "Chapter 3: Arrays", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 3, heading: "Chapter 4: Abstract Data Types", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { 
                id: 4, 
                heading: "Chapter 5: Stack", 
                placeholder: `A Stack is a linear data structure operating on the Last-In, First-Out (LIFO) paradigm. This implies that elements appended most recently are the primary items retrieved next.\n\nCore Stack Operations:\n• Push: Appends an element to the peak position of the data structure.\n• Pop: Extracts and discards the element situated at the top boundary.\n• Top / Peek: Observes the item located at the highest index without altering structural state.\n• IsEmpty: Validates whether data elements are present within the active constraints.\n\nImplementation Framework Sample:\n\nclass CourseworkStack {\nprivate:\n    int storage[100];\n    int topIndex;\npublic:\n    CourseworkStack() { topIndex = -1; }\n    \n    void push(int dataValue) {\n        if (topIndex >= 99) return;\n        storage[++topIndex] = dataValue;\n    }\n    \n    void pop() {\n        if (topIndex < 0) return;\n        topIndex--;\n    }\n};`
            },
            { id: 5, heading: "Chapter 6: Queue", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 7, heading: "Chapter 7: Sorting Algorithms", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 8, heading: "Chapter 8: Searching Algorithms", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 9, heading: "Chapter 9: Linked List", placeholder: "Content details pending configuration. Select this chapter above to add course logs." },
            { id: 10, heading: "Chapter 10: Tree", placeholder: "Content details pending configuration. Select this chapter above to add course logs." }
        ];

        let userContent = JSON.parse(localStorage.getItem('muaz_portfolio_records')) || {};

        function renderPortfolioDisplay() {
            const wrapper = document.getElementById('portfolio-container');
            wrapper.innerHTML = '';

            systemChapters.forEach(chap => {
                const textValue = userContent[chap.id] || chap.placeholder;
                const isCustom = !!userContent[chap.id];

                wrapper.innerHTML += `
                    <div class="chapter-card" id="card-block-${chap.id}">
                        <h2>${chap.heading}</h2>
                        <div class="chapter-content">${escapeHTML(textValue)}</div>
                        ${isCustom ? `<button class="btn-clear" onclick="clearTargetBlock(${chap.id})">Reset to Default</button>` : ''}
                    </div>
                `;
            });
        }

        function saveChapterData() {
            const selectorIndex = document.getElementById('chapter-select').value;
            const textInput = document.getElementById('chapter-body').value;

            if(!textInput.trim()) {
                alert('Please type or paste some text before updating.');
                return;
            }

            userContent[selectorIndex] = textInput;
            localStorage.setItem('muaz_portfolio_records', JSON.stringify(userContent));
            
            document.getElementById('chapter-body').value = '';
            renderPortfolioDisplay();
            document.getElementById(`card-block-${selectorIndex}`).scrollIntoView({ behavior: 'smooth' });
        }

        function clearTargetBlock(targetId) {
            if(confirm('Reset this chapter block text?')) {
                delete userContent[targetId];
                localStorage.setItem('muaz_portfolio_records', JSON.stringify(userContent));
                renderPortfolioDisplay();
            }
        }

        function escapeHTML(str) {
            return str.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;");
        }

        renderPortfolioDisplay();
    </script>
</body>
</html>
