Website for a future business idea. This is meant to stretch my ability to learn and is a large undertaking. I have installed Material, Tailwind, Express, and Pug so far. The base webpage will be implemented in HTML, plain JS, and Tailwind CSS. Material UI has been installed and prepped and ocne the page is finished, it will be converted to a React project to mimic an actual project that might be given in a work environment. Material UI will utilize React, Tailwind, and Material's library is the interface between them. React DOM has been installed into the project along with Material, but it is not loaded yet until functionality is finished.

Notes for website so far:

IT WILL NOT RUN ON EXPRESS CURRENTLY. I need to fix the pathing. In order to run, I learned about several plugins and the format can currently be checked using Live Server. Do not attempt to run on Localhost 5000 or it WILL throw an error.

Notes to run the service:
- You can use the command: npx tailwindcss -i ./public/css/input.css -o ./dist/output.css --watch creates output.css
- You can use the command: npx tailwindcss -i ./public/css/input.css -o ./dist/styles.css --watch to run a different stlyesheet named styles.css
- Install Live Server plugin


To actually start the preview use: "npm run dev" then select Run Live Server.

Observations while coding for personal improvement:
- VS Code has a tendency to corrupt file paths.
- When inserting a background image, do not put the margins on the section divider or the div, use padding to avoid large white margins.
- Inserting custom CSS into the output.css file will overwrite

Implementation Requirements:
- It will be a single page
- Clicking a buttons in the navigation bar should skip the user to the appropriate section without scrolling.
- Optional, the navbar scrolls with the user (currently static)
- Clicking on the login button will open a modal with the account information
- The only other view will be the account page
- Users should be able to view menu items
- Menu items should dynamically update from a database of items

Problems I encountered:
- Tailwind did not want to configure italics or a border nor did column-row functionality work. It seemed like the classes were only being used part of the time and only in places where I had copied the git repository from my desktop onto my laptop. In other words, added code on my laptop did not have functionality.
    + Attempts at a solution:
        - Stackoverflow suggested setting tailwind to "border border-solid". This had no effect.
        - I copied solutions for creating a card both off of Material UI's website and Tailwind CSS's website. This also had no effect. - I suspected a missing closing tab. This was also not the problem.
    + Most likely issue:
        - Node.js appears to have been uninstalled from this laptop as using the commands node -v and npm cli to attempt reinstallation of all packages resultes in a command not found. Solution is like re-installing node.