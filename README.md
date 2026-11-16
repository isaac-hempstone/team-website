# team-website

live site:https://isaac-hempstone.github.io/team-website/

Team:
Isaac Hempstone COM/3489/26 GITHUB USERNAME:isaac-hempstone<br/>
Patrick

Reflection Questions

1. The menu toggle is a "<button>", not a clickable "<div>". Name two things you would lose with a "<div>", and who would be affected.

A "<div>" does not automatically support keyboard interaction or have button semantics. This would make the menu harder to use for keyboard users and people using screen readers. A "<button>" provides built-in keyboard support and accessibility.

2. What would break if you removed "defer" from the "<script>" tag in "<head>"? Explain why, in terms of how the browser parses HTML.

Without "defer", the browser would stop parsing the HTML while it downloads and executes the JavaScript. The script might run before the HTML elements are loaded, causing JavaScript functions that access those elements to fail. Using "defer" allows the browser to finish parsing the HTML before executing the script.

3. "renderProjects" uses "textContent" rather than "innerHTML". What could go wrong with "innerHTML" if project titles were typed in by visitors?

Using "innerHTML" with visitor input could allow harmful HTML or JavaScript to be inserted into the webpage. This could create a security problem called Cross-Site Scripting (XSS). Using "textContent" displays the input as plain text, making it safer.

4. Your form checks its input with JavaScript. Why will the server still need to validate the same data once the form is connected to one?

JavaScript validation happens in the browser and can be bypassed by users. Server-side validation is necessary to make sure the submitted information is correct and safe. It protects the application and its data from invalid or harmful submissions.

5. Your theme choice follows you from Home to Contact, but not from a double-clicked file to Live Server. Explain this using the idea of an origin.

An origin is made up of a website's protocol, domain name and port number. Home and Contact share the same origin when opened through Live Server, so they can access the same saved theme preference. Opening a file directly uses a different origin from Live Server, so the saved preference may not be shared.

6. Name something duplicated across your HTML pages. What problem does that duplication cause, and how might it be avoided?

The navigation menu and footer are duplicated across the HTML pages. This can make updating the website difficult because the same changes must be made on every page. This duplication can be avoided by using reusable components or shared templates.
