# Convex Schema Tools

Convex Schema Tools is a minimal web app for visualizing Convex database schemas and converting SQL queries to Convex code. It helps developers and teams:

- Instantly generate interactive Entity-Relationship Diagrams (ERD) from Convex TypeScript schemas
- Export diagrams as PNG images (including all table overlays and relationships)
- Convert SQL queries (SELECT, INSERT, UPDATE, DELETE) into Convex query/mutation code
- Explore and share database structure visually

## Features

- **Schema → Diagram**: Paste your Convex schema (TypeScript) and generate a beautiful, interactive ERD. Tables and relationships are auto-detected and rendered.
- **Zoom & Pan**: Use mouse or the + / - buttons to zoom in/out and pan the diagram.
- **Export as PNG**: Download a PNG image of the diagram exactly as you see it, including all table overlays and arrows.
- **SQL → Convex**: Paste a SQL query and get a Convex query/mutation as a starting point for your backend code.
- **Minimal UI**: Inspired by Notion, with a focus on clarity and usability.

## How to Use

1. **Open the app in your browser.**
2. **Schema to Diagram:**
   - Go to the "Schema → Diagram" tab.
   - Paste your Convex schema (TypeScript) into the textarea.
   - Click "Generate Diagram".
   - The ERD will appear below. You can zoom, pan, and explore.
   - Click "+" or "-" to zoom in/out. Click "Fit View" to center everything.
   - Click "Export PNG" to download the diagram as an image.
3. **SQL to Convex:**
   - Go to the "SQL → Convex" tab.
   - Paste a SQL query (SELECT, INSERT, UPDATE, DELETE).
   - Click "Convert to Convex" to see the generated Convex code.

## Technologies Used

- [Cytoscape.js](https://js.cytoscape.org/) for graph rendering
- [html2canvas](https://html2canvas.hertzen.com/) for PNG export
- Vanilla JavaScript, HTML, and CSS (no build step required)

## Tips & Limitations

- The schema parser is designed for Convex TypeScript schemas using `defineTable` and `defineSchema`.
- The ERD layout is optimized for clarity, but very large schemas may require manual zoom/pan.
- PNG export captures the diagram as seen on screen, including all overlays and arrows.
- SQL to Convex conversion is a starting point and may require manual adjustment for complex queries.
