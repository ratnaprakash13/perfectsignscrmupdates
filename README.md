[README.md](https://github.com/user-attachments/files/29780495/README.md)
# June 2026 Invoice Work Timeline UI

This is a standalone, single-page responsive timeline application specifically populated with daily work logs for **June 2026** to support your client invoice audits. 

## Calendar Configuration (June 2026)
- **Work Days**: All 21 weekdays (Mondays through Fridays) in June 2026 are individually documented.
- **Exclusions**: Weekend days (Saturdays and Sundays) and the Canadian holiday **Saint-Jean-Baptiste Day** (Wednesday, June 24, 2026) are excluded.
- **Detailed Content**: Includes backend configurations (.NET 10 Web API, PostgreSQL whitelisting, IIS ARR proxy config), frontend installations (Node.js, Bootstrap 5, Vite React scaffolding), and bug fixes.

## Customization
To change the daily updates or project details, simply open `index.html` in a text editor (like Notepad, VS Code) and customize the HTML text:

1. **Header Details**: Edit the header values at lines 270-275 to change the project title or client name.
2. **Timeline Items**: Add, edit, or copy-paste the `timeline-item` blocks (lines 292-800+) to add or change daily updates.

## How to Host on IIS
1. Copy the `index.html` file onto your Windows Server.
2. Create a new Website in IIS pointing to the directory containing `index.html`.
3. Give your client the URL!
