HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Typography Showcase</title>
    <!-- Google Fonts Import -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Header Section -->
    <header class="page-header">
        <h1>Typography Showcase</h1>
        <p class="subtitle">Exploring font pairings, scales, weights, and text styling properties.</p>
    </header>

    <main class="container">

        <!-- Section 1: Heading Styles -->
        <section class="typography-section">
            <h2>1. Heading Styles</h2>
            <p class="section-desc">Headings use <em>Playfair Display</em> with distinct weights, font sizes, and custom letter spacing.</p>
            
            <h1 class="demo-h1">Heading 1 — Majestic Headline (Bold 700)</h1>
            <h2 class="demo-h2">Heading 2 — Subheading Title (Semi-Bold 600)</h2>
            <h3 class="demo-h3">Heading 3 — Section Header (Regular 400)</h3>
            <h4 class="demo-h4">Heading 4 — Minor Caption (Italicized)</h4>
        </section>

        <!-- Section 2: Paragraph Styles -->
        <section class="typography-section">
            <h2>2. Paragraph Styles</h2>
            <p class="section-desc">Paragraphs use <em>Inter</em> with optimized line-heights and text alignments for readability.</p>
            
            <p class="demo-left"><strong>Left-Aligned:</strong> This paragraph demonstrates standard left-aligned text styling. Notice the comfortable line-height and letter spacing which improves readability across multi-line blocks of digital content.</p>
            
            <p class="demo-center"><strong>Centered:</strong> This paragraph uses centered text alignment, commonly utilized for blockquotes, banners, or call-to-action headers.</p>
            
            <p class="demo-justify"><strong>Justified:</strong> This paragraph is justified across the container width to create clean, block-like vertical margins on both sides, resembling traditional print layouts.</p>
        </section>

        <!-- Section 3: Text Emphasis -->
        <section class="typography-section">
            <h2>3. Text Emphasis</h2>
            <p class="section-desc">Demonstrating font styles, text decorations, weights, and inline variations.</p>
            
            <p class="demo-emphasis">
                This sentence contains <span class="fw-bold">bold weighted text</span>, <span class="font-italic">italicized expressions</span>, <span class="text-underline">underlined keywords</span>, and <span class="text-strike">outdated strikethrough references</span> to show inline styling flexibility.
            </p>
        </section>

    </main>

    <footer>
        <p>&copy; 2026 Typography Showcase Practice</p>
    </footer>

</body>
</html>

CSS
/* Global Reset & Typography Setup */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Inter', sans-serif; /* Body font family */
    background-color: #f8f9fa;
    color: #212529;
    line-height: 1.7; /* Adjusted line-height for readability */
    padding: 30px 20px;
}

/* Page Header */
.page-header {
    text-align: center;
    margin-bottom: 40px;
}

.page-header h1 {
    font-family: 'Playfair Display', serif; /* Heading font family */
    font-size: 2.8rem;
    font-weight: 700;
    color: #1a1a1a;
    letter-spacing: 1px;
    margin-bottom: 8px;
}

.subtitle {
    font-size: 1.1rem;
    color: #6c757d;
    font-weight: 300;
}

/* Main Container Layout */
.container {
    max-width: 850px;
    margin: 0 auto;
}

/* Sections */
.typography-section {
    background: #ffffff;
    padding: 30px;
    margin-bottom: 30px;
    border-radius: 10px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.04);
}

.typography-section h2 {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem;
    color: #2c3e50;
    margin-bottom: 8px;
    border-bottom: 2px solid #e9ecef;
    padding-bottom: 8px;
}

.section-desc {
    font-size: 0.95rem;
    color: #6c757d;
    margin-bottom: 20px;
}

/* 1. Heading Styles Variations */
.demo-h1 {
    font-family: 'Playfair Display', serif;
    font-size: 2.2rem;
    font-weight: 700;
    letter-spacing: 0.5px;
    color: #2c3e50;
    margin-bottom: 12px;
}

.demo-h2 {
    font-family: 'Playfair Display', serif;
    font-size: 1.8rem;
    font-weight: 600;
    letter-spacing: 0.3px;
    color: #34495e;
    margin-bottom: 10px;
}

.demo-h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.4rem;
    font-weight: 400;
    color: #7f8c8d;
    margin-bottom: 8px;
}

.demo-h4 {
    font-family: 'Playfair Display', serif;
    font-size: 1.1rem;
    font-style: italic;
    font-weight: 400;
    color: #95a5a6;
    margin-bottom: 5px;
}

/* 2. Paragraph Styles Variations */
.demo-left {
    text-align: left;
    margin-bottom: 15px;
}

.demo-center {
    text-align: center;
    background-color: #f1f3f5;
    padding: 12px;
    border-radius: 6px;
    margin-bottom: 15px;
}

.demo-justify {
    text-align: justify;
    margin-bottom: 15px;
}

/* 3. Text Emphasis Styles */
.demo-emphasis {
    font-size: 1.05rem;
}

.fw-bold {
    font-weight: 600;
    color: #e67e22;
}

.font-italic {
    font-style: italic;
    color: #8e44ad;
}

.text-underline {
    text-decoration: underline;
    text-decoration-color: #3498db;
    text-underline-offset: 3px;
}

.text-strike {
    text-decoration: line-through;
    color: #95a5a6;
}

/* Footer */
footer {
    text-align: center;
    color: #adb5bd;
    font-size: 0.9rem;
    margin-top: 40px;
}