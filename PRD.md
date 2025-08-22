Product Requirements Document (PRD)
===================================

**Project:** LED Lights Payback (ROI) Calculator**Technology:** HTML with Inline CSS & JavaScript (single file, embeddable)**Prepared For:** \[Client Name / Company\]**Prepared By:** \[Your Name / Agency\]**Date:** \[Insert Date\]

**1\. Introduction**
--------------------

### Purpose

Develop a **web-based LED Lights Payback Calculator** that runs fully in the browser, requires no backend, and is delivered as a **single HTML file with inline JavaScript and CSS**.

This ensures maximum compatibility and ease of embedding into **WordPress** or any other CMS without plugins or extra uploads.

**2\. Scope**
-------------

### In Scope

*   Self-contained calculator (inline JS + CSS).
    
*   Two sections: **Baseline** (manual inputs) vs **Proposed** (drop-down LED products).
    
*   Core outputs: Initial cost, annual energy usage, annual cost, annual savings, payback period.
    
*   Dropdown populated with client’s **product catalog**.
    
*   Branding (logo + colors).
    
*   Responsive design.
    
*   Print/Export results.
    

### Out of Scope

*   External CSS/JS files.
    
*   Backend/database integration.
    
*   Multi-language or localization.
    

**3\. User Stories**
--------------------

1.  **As a customer**, I want to enter baseline values manually to simulate my current setup.
    
2.  **As a customer**, I want to choose from the client’s LED fixtures dropdown (auto-filling wattage).
    
3.  **As a customer**, I want to see clear comparison results (costs, usage, savings).
    
4.  **As a customer**, I want to print/export the results for reference.
    
5.  **As the client**, I want to easily embed the calculator in WordPress with a single copy-paste.
    

**4\. Functional Requirements**
-------------------------------

### Inputs

*   Electricity Rate (cents/kWh).
    
*   Operation Hours (hours/day).
    
*   Baseline: Quantity, Watts per luminaire, Cost per luminaire.
    
*   Proposed: Dropdown (pre-defined fixtures), Quantity, Cost per luminaire.
    

### Outputs

*   Initial Cost.
    
*   Annual Energy Usage (kWh).
    
*   Annual Energy Cost.
    
*   Annual Savings.
    
*   Payback Period.
    

### Calculations

1.  Quantity×Watts×Hours per Day×365÷1000\\text{Quantity} \\times \\text{Watts} \\times \\text{Hours per Day} \\times 365 \\div 1000Quantity×Watts×Hours per Day×365÷1000
    
2.  Annual Energy×Rate100\\text{Annual Energy} \\times \\frac{\\text{Rate}}{100}Annual Energy×100Rate​
    
3.  Quantity×Cost per Fixture\\text{Quantity} \\times \\text{Cost per Fixture}Quantity×Cost per Fixture
    
4.  Baseline Cost−Proposed Cost\\text{Baseline Cost} - \\text{Proposed Cost}Baseline Cost−Proposed Cost
    
5.  Proposed Initial CostAnnual Savings\\frac{\\text{Proposed Initial Cost}}{\\text{Annual Savings}}Annual SavingsProposed Initial Cost​
    

**5\. Design Requirements**
---------------------------

### Layout

*   **Header:** Logo + title.
    
*   **Input Section:**
    
    *   Left: Baseline form.
        
    *   Right: Proposed form.
        
*   **Results Section:** Side-by-side table + highlighted savings.
    
*   **Footer:** Print/Export + disclaimer.
    

### Styling

*   Minimalist, clean design.
    
*   Inline CSS tag inside <head>.</div></li><li class="slate-li"><div style="position:relative">Responsive grid using pure CSS (no frameworks).</div></li></ul><h2 class="slate-h2"><strong class="slate-bold">6. Technical Requirements</strong></h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Delivery Format:</strong> Single .html file with inline CSS and JavaScript.</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Technology:</strong></div><ul class="slate-ul"><li class="slate-li"><div style="position:relative">HTML5 (structure)</div></li><li class="slate-li"><div style="position:relative">Inline CSS (inside <style>)</div></li><li class="slate-li"><div style="position:relative">Inline Vanilla JS (inside <script>)</div></li></ul></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Embedding:</strong></div><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Can be pasted directly into WordPress via "Custom HTML" block.</div></li><li class="slate-li"><div style="position:relative">No dependencies, no external requests.</div></li></ul></li></ul><h2 class="slate-h2"><strong class="slate-bold">7. Product Catalog (Dropdown)</strong></h2><h3 class="slate-h3">Fixtures to Include</h3><ul class="slate-ul"><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Tundra Area Light</strong> – 70W, 100W, 150W, 200W, 240W, 300W</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Orbix Round UFO Light</strong> – 70W, 100W, 150W, 180W, 200W, 240W</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Alpine LED Wall Pack Light</strong> – 80W, 100W, 120W</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Raven Backlit Flat Panel Light 2x4</strong> – 30W, 40W, 50W, 60W, 72W</div></li><li class="slate-li"><div style="position:relative"><strong class="slate-bold">Raven Backlit Flat Panel Light 2x2/1x4</strong> – 15W, 20W, 25W, 30W, 40W</div></li></ul><h2 class="slate-h2"><strong class="slate-bold">8. Deliverables</strong></h2><ol class="slate-ol"><li class="slate-li"><div style="position:relative">A <strong class="slate-bold">single HTML file</strong> containing all markup, styling, and scripts.</div></li><li class="slate-li"><div style="position:relative">Easy embedding instructions for WordPress.</div></li><li class="slate-li"><div style="position:relative">Documentation of calculations and fields.</div></li></ol><h2 class="slate-h2"><strong class="slate-bold">9. Risks & Assumptions</strong></h2><ul class="slate-ul"><li class="slate-li"><div style="position:relative">Users may input unrealistic values (basic validation included).</div></li><li class="slate-li"><div style="position:relative">Assumes client provides final logo + branding hex codes.</div></li><li class="slate-li"><div style="position:relative">Browser support: Chrome, Safari, Edge, Firefox (latest versions).</div></li></ul><p class="slate-paragraph"></p></x-turndown>