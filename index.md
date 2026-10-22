HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Typography Showcase</title>
  <meta name="description" content="A demonstration of complementary Google Fonts and web typography styling.">
  <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>✍️</text></svg>">

  <!-- Step 1: Import 2 Complementary Google Fonts (Playfair Display + Inter) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:ital,wght@0,300;0,400;0,600;0,700;1,400&family=Playfair+Display:ital,wght@0,600;0,700;0,900;1,400;1,700&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="typography.css">
</head>
<body>

  <header class="showcase-header">
    <p class="eyebrow">Design System &middot; Specimen 01</p>
    <h1>Web Typography Showcase</h1>
    <p class="subtitle">Exploring typographic hierarchy, Google Fonts pairing, weights, and spatial rhythm.</p>
  </header>

  <main class="showcase-container">

    <!-- Section 1: Heading Styles -->
    <section class="showcase-section">
      <div class="section-badge">Section 01</div>
      <h2>Heading Styles</h2>
      <p class="section-intro">Display headers set in <em>Playfair Display</em> with tight letter-spacing and distinct scale ratios.</p>

      <div class="specimen-block">
        <h1 class="sample-h1">Level 1 Heading &mdash; 2.5rem (Weight 900)</h1>
        <h2 class="sample-h2">Level 2 Heading &mdash; 1.85rem (Weight 700)</h2>
        <h3 class="sample-h3">Level 3 Heading &mdash; 1.35rem (Weight 600)</h3>
        <h4 class="sample-h4">Level 4 Small Caps Subhead &mdash; 0.95rem</h4>
      </div>
    </section>

    <!-- Section 2: Paragraph Styles -->
    <section class="showcase-section">
      <div class="section-badge">Section 02</div>
      <h2>Paragraph Styles</h2>
      <p class="section-intro">Body text rendered in <em>Inter</em> with custom line heights, font sizes, and alignments.</p>

      <div class="specimen-block">
        <p class="text-lead">
          <strong>Lead Paragraph:</strong> Good typography establishes a visual hierarchy that guides the reader effortlessly through content. When font pairings harmonize, reading fatigue diminishes and retention improves.
        </p>

        <p class="text-standard">
          <strong>Standard Body (Left-Aligned):</strong> The font-size for standard reading body copy sits comfortably between 16px and 18px. A generous line-height of 1.7 ensures that the eye can track across the line length without inadvertently jumping back or re-reading text lines.
        </p>

        <p class="text-centered">
          <strong>Centered Callout:</strong> "Typography is the craft of endowing human language with a durable visual form."
        </p>

        <p class="text-justified">
          <strong>Justified Paragraph:</strong> In editorial and print-inspired web designs, justified text aligns evenly along both left and right margins. It requires balanced line-height and letter-spacing to prevent erratic spacing gaps between words.
        </p>
      </div>
    </section>

    <!-- Section 3: Text Emphasis -->
    <section class="showcase-section">
      <div class="section-badge">Section 03</div>
      <h2>Text Emphasis</h2>
      <p class="section-intro">Applying text-decoration, font-style, transformed casing, and weighted accents.</p>

      <div class="specimen-block emphasis-grid">
        <div class="emphasis-item">
          <span class="label">Font Style (Italics)</span>
          <p class="style-italic">Emphasizing reflective thought through graceful italic serif phrasing.</p>
        </div>

        <div class="emphasis-item">
          <span class="label">Text Decoration (Underline &amp; Offset)</span>
          <p><a href="#" class="style-underline">Accent link with custom underline offset and thickness</a></p>
        </div>

        <div class="emphasis-item">
          <span class="label">Text Decoration (Line-Through)</span>
          <p class="style-strikethrough">Original regular subscription price: $99 / yr</p>
        </div>

        <div class="emphasis-item">
          <span class="label">Tracked Uppercase &amp; Weights</span>
          <p class="style-tracking">Curated editorial design standard</p>
        </div>
      </div>
    </section>

  </main>

  <footer class="showcase-footer">
    <p>&copy; 2026 Typography Showcase &middot; Playfair Display &amp; Inter</p>
  </footer>

</body>
</html>

CSS
/* =========================================================
   Reset & Baseline
   ========================================================= */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* =========================================================
   Step 2: Base Body Setup (Inter)
   Step 3 & 5: Font size, weight, line-height
   ========================================================= */
body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  background-color: #fbfbfa;
  color: #2b2d42;
  font-size: 1rem;       /* 16px */
  font-weight: 400;
  line-height: 1.7;      /* Generous line-height */
  padding: 40px 20px;
}

/* =========================================================
   Step 2: Headings Setup (Playfair Display)
   Step 5: letter-spacing & line-height adjustments
   ========================================================= */
h1, h2, h3, h4 {
  font-family: 'Playfair Display', Georgia, serif;
  color: #1a1a24;
  line-height: 1.25;
  letter-spacing: -0.02em;
}

/* Header Area */
.showcase-header {
  max-width: 860px;
  margin: 0 auto 48px auto;
  text-align: center;
}

.eyebrow {
  font-size: 0.8rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: #8d99ae;
  margin-bottom: 8px;
}

.showcase-header h1 {
  font-size: 2.75rem;
  font-weight: 900;
  margin-bottom: 12px;
}

.subtitle {
  font-size: 1.15rem;
  color: #64748b;
  max-width: 580px;
  margin: 0 auto;
}

/* Page Container */
.showcase-container {
  max-width: 860px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  gap: 36px;
}

/* Section Containers */
.showcase-section {
  background-color: #ffffff;
  border: 1px solid #e9ecef;
  border-radius: 12px;
  padding: 36px;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.03);
}

.section-badge {
  font-size: 0.75rem;
  font-weight: 700;
  letter-spacing: 0.1em;
  color: #2563eb;
  text-transform: uppercase;
  margin-bottom: 6px;
}

.showcase-section h2 {
  font-size: 1.75rem;
  font-weight: 700;
  margin-bottom: 8px;
}

.section-intro {
  font-size: 0.95rem;
  color: #6c757d;
  margin-bottom: 24px;
  padding-bottom: 14px;
  border-bottom: 1px solid #f1f3f5;
}

.specimen-block {
  display: flex;
  flex-direction: column;
  gap: 18px;
}

/* =========================================================
   Section 1: Heading Scale Variants (Sizes & Weights)
   ========================================================= */
.sample-h1 {
  font-size: 2.25rem;
  font-weight: 900;
  letter-spacing: -0.03em;
}

.sample-h2 {
  font-size: 1.75rem;
  font-weight: 700;
  letter-spacing: -0.02em;
}

.sample-h3 {
  font-size: 1.35rem;
  font-weight: 600;
  color: #3f37c9;
}

.sample-h4 {
  font-size: 0.95rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: #6c757d;
}

/* =========================================================
   Section 2: Paragraph Styles & text-align
   ========================================================= */
.text-lead {
  font-size: 1.2rem;
  font-weight: 300;
  line-height: 1.75;
  color: #1e293b;
}

.text-standard {
  font-size: 1rem;
  line-height: 1.7;
  text-align: left;
}

.text-centered {
  text-align: center;
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-size: 1.25rem;
  color: #1e3a8a;
  background-color: #f8faff;
  padding: 16px 20px;
  border-radius: 8px;
  border-left: 4px solid #2563eb;
}

.text-justified {
  text-align: justify;
  font-size: 0.95rem;
  line-height: 1.65;
  color: #475569;
}

/* =========================================================
   Section 3: Text Emphasis, text-decoration & font-style
   ========================================================= */
.emphasis-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 18px;
}

.emphasis-item {
  background-color: #f8fafc;
  padding: 16px 18px;
  border-radius: 8px;
  border: 1px solid #edf2f7;
}

.emphasis-item .label {
  display: block;
  font-size: 0.72rem;
  font-weight: 700;
  color: #94a3b8;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 6px;
}

.style-italic {
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-weight: 400;
  font-size: 1.05rem;
  color: #334155;
}

.style-underline {
  color: #2563eb;
  font-weight: 600;
  text-decoration: underline;
  text-decoration-thickness: 2px;
  text-underline-offset: 4px;
  text-decoration-color: #93c5fd;
  transition: text-decoration-color 0.2s ease;
}

.style-underline:hover {
  text-decoration-color: #2563eb;
}

.style-strikethrough {
  text-decoration: line-through;
  text-decoration-color: #ef4444;
  color: #94a3b8;
}

.style-tracking {
  text-transform: uppercase;
  letter-spacing: 0.18em;
  font-size: 0.82rem;
  font-weight: 700;
  color: #1e293b;
}

/* Footer */
.showcase-footer {
  text-align: center;
  margin-top: 48px;
  font-size: 0.85rem;
  color: #94a3b8;
}