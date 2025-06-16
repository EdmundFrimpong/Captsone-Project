<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Capstone Project Summary</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@700&display=swap');

        body {
            font-family: 'Montserrat', sans-serif;
            background: #f9f9f9;
            margin: 0;
            padding: 0;
            color: #333;
            font-size: 18px; /* Increased base font size for overall page */
        }

        header {
            background-color: #ff8c00;
            color: white;
            text-align: center;
            padding: 30px 20px;
        }

        .container {
            max-width: 1200px; /* Adjusted for wider content */
            margin: 40px auto;
            padding: 0 20px;
        }

        section {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            margin-bottom: 30px;
            padding: 30px;
        }

        h2 {
            color: #ff8c00;
            margin-top: 0;
        }

        p, ul {
            font-size: 1.1em; /* Increased specific font size for paragraphs and lists relative to body */
            line-height: 1.6;
        }

        ul {
            padding-left: 20px;
        }

        footer {
            text-align: center;
            color: #777;
            padding: 20px 0;
        }

        /* Responsive iframe styling */
        .iframe-container {
            position: relative;
            width: 100%;
            padding-bottom: 75%; /* 4:3 aspect ratio (450/600 = 0.75) */
            height: 0;
            overflow: hidden;
            margin-top: 20px;
            margin-bottom: 20px;
        }

        .iframe-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Capstone Project Overview</h1>
        <p>A Deep Dive Into My Final Project</p>
    </header>

    <div class="container">
        <section id="summary">
            <h2>1. Project Summary</h2>
            <p>
                This capstone project centers on credit scoring and financial behavior analysis using a structured financial transactions dataset.
                The objective is to analyze customer-level data related to credit card usage, outstanding debts, and reported income
                in order to identify patterns that influence creditworthiness. The findings are intended to help financial institutions
                enhance decision-making around credit approvals and risk profiling.
            </p>
        </section>

        <section id="dataset">
            <h2>2. Where the Dataset Came From</h2>
            <p>
                The dataset used in this project is titled
                <strong>Financial Transactions Dataset: Analytics</strong>, sourced from
                <a href="https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets" target="_blank">Kaggle</a>.
                This comprehensive financial dataset combines transaction records, customer information, and card data
                from a banking institution, spanning across the 2010s decade. It is designed for various analytical
                purposes including synthetic fraud detection, customer behavior analysis, and expense forecasting.
            </p>
        </section>

        <section id="tools">
            <h2>3. Tools Used</h2>
            <ul>
                <li><strong>MySQL</strong> – for storing, cleaning, and querying the dataset efficiently using SQL.</li>
                <li><strong>Excel</strong> – for initial data exploration, filtering, and performing quick calculations or summaries.</li>
                <li><strong>Looker Studio</strong> – to build interactive visualizations and dashboards that clearly present insights.</li>
            </ul>
        </section>

        <section id="steps">
            <h2>4. Steps Taken</h2>
            <ul>
                <li><strong>Data Acquisition & Database Setup:</strong> Loaded the raw Kaggle dataset into a MySQL database. Designed and implemented appropriate schemas for efficient storage and querying.</li>
                <li><strong>Data Cleaning & Transformation:</strong> Conducted thorough data cleaning, addressing missing values, correcting data types, and handling inconsistencies. Performed feature engineering to derive new metrics (e.g., Debt-to-Income ratio, average spending per user) crucial for analysis.</li>
                <li><strong>Exploratory Data Analysis (EDA):</strong> Used Excel for initial high-level summaries and pattern identification. Leveraged SQL queries in MySQL to perform deeper statistical analysis, aggregation (like average income by age group, credit score by number of credit cards), and segmentation of the user base.</li>
                <li><strong>Key Question Formulation:</strong> Defined specific business questions (e.g., How Does Income Change With Age? Is Debt Lower after Retirement? Is there a relationship between credit score and debt or spending?) to guide the analysis and ensure actionable insights.</li>
                <li><strong>Visualization & Dashboarding:</strong> Utilized Looker Studio to create interactive dashboards. These visualizations translated complex data trends into easily digestible charts, illustrating relationships such as income vs. age and credit score vs. debt/spending.</li>
                <li><strong>Insight Generation & Storytelling:</strong> Interpreted the visual and statistical findings to derive actionable business insights. Focused on clear, concise communication of results, highlighting key patterns and implications for financial institutions.</li>
            </ul>
        </section>

        <section id="dashboard">
            <h2>5. Interactive Dashboard</h2>
            <p>Explore the key findings and interactive visualizations below. Use the filters and controls within the dashboard to dive deeper into the data.</p>
            <div class="iframe-container">
                <iframe src="https://lookerstudio.google.com/embed/reporting/f2e838d9-ea0c-4aa3-bf2a-10e3a9f41987/page/7Y5NF" frameborder="0" style="border:0" allowfullscreen sandbox="allow-storage-access-by-user-activation allow-scripts allow-same-origin allow-popups allow-popups-to-escape-sandbox"></iframe>
            </div>
        </section>

        <section id="findings">
            <h2>6. Key Findings & Insights</h2>
            <p>Through comprehensive analysis, several key insights into customer financial behavior and creditworthiness were uncovered:</p>
            <ul>
                <li><strong>Income Stability Across Working Ages:</strong> Contrary to typical patterns, average income within our dataset remained relatively stable across prime working age groups (18-65), showing a plateau rather than a distinct mid-career peak. A significant decline was observed only after age 65, consistent with retirement.</li>
                <li><strong>Demographic Split by Retirement Status:</strong> The user base is predominantly non-retired (75%), with a significant portion (6.55%) actively approaching retirement within 5 years. This highlights varying financial priorities across the user lifecycle.</li>
                <li><strong>Credit Card Ownership & Score Relationship:</strong> Owning a moderate number of credit cards (e.g., 3-8 in our dataset) was associated with the highest average credit scores, suggesting responsible multi-account management. However, having an excessive number of cards (e.g., 9+) appeared detrimental to credit scores.</li>
                <li><strong>Complex Credit Score-Debt Relationship:</strong> No strong direct correlation was found between credit score and total debt. High debt levels were observed across various credit score ranges, indicating that factors beyond score, such as income and financial obligations, play a significant role.</li>
                <li><strong>Credit Score Not a Spending Predictor:</strong> Similarly, credit score did not show a strong linear relationship with individual spending habits. Average spending per user fluctuated independently of credit score, suggesting spending is more influenced by income and lifestyle choices.</li>
            </ul>
            <p>These findings provide actionable intelligence for financial institutions to refine their credit risk models, tailor product offerings, and improve customer segmentation strategies.</p>
        </section>
    </div>

    <footer>
        <p>&copy; 2025 Your Name | Capstone Project</p>
    </footer>
</body>
</html>