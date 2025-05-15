PageRank Explainer: An Interactive Journey with Markov Chains
This project is an educational website designed to explain the concepts of Markov Chains and Google's PageRank algorithm. It features an interactive demonstration where users can visualize how PageRank is calculated by simulating a random surfer on a small network of interconnected pages. User clicks directly influence and display the mathematical state transitions and probability distributions.


Features
Educational Content: Clear explanations of Markov Chains, the PageRank algorithm, and the underlying mathematics.
Interactive Demo:
Visualize a small web graph with clickable nodes (pages).
See the current page of the simulated surfer highlighted.
Observe the PageRank vector (probability distribution) update with each step or click.
View the Google Matrix used for calculations.
Manually step through iterations or let the simulation run.
Reset the simulation to its initial state.
Responsive Design: The website is designed to be usable on different screen sizes.
Technology Stack
Frontend: React (with Vite as the build tool)
Programming Language: JavaScript (JSX for React components)
Styling: Tailwind CSS
Package Manager: pnpm
Core Logic: Custom JavaScript functions for Markov Chain and PageRank calculations.
Prerequisites
Before you can run this project locally, you need to have the following software installed on your system:
Node.js: (LTS version recommended, e.g., v18.x or v20.x). Download from nodejs.org. This will also install npm.
pnpm: The project uses pnpm for package management. Install it globally using npm:
bash
npm install -g pnpm
Git: (Optional, if you plan to clone from a repository, but not strictly necessary if you have the source code zip).
Getting Started
Follow these steps to get the project running on your local machine:
Obtain the Source Code:
If you have the pagerank_explainer_source_code.zip file, extract it to a folder on your computer.
This will create a directory named pagerank_explainer.
Navigate to the Project Directory:
Open your terminal or command prompt and change to the project's root directory:
bash
cd path/to/pagerank_explainer
Install Dependencies:
Run the following command to install all the necessary project dependencies using pnpm:
bash
pnpm install
Note on Build Scripts: During installation, pnpm might show a warning about ignored build scripts (e.g., for esbuild). If it does, run the command it suggests to approve them:
bash
pnpm approve-builds
Then, you might need to run pnpm install again if the initial install was interrupted.
Run the Development Server:
Once the dependencies are installed, start the local development server:
bash
pnpm run dev
This will compile the application and serve it locally. The terminal will typically show a message like:
VITE vX.Y.Z  ready in XXX ms

➜  Local:   http://localhost:5173/
View in Browser:
Open your web browser and go to the URL http://localhost:5173/ (or whatever URL is shown in your terminal ).
You should see the PageRank Explainer website running.
Available Scripts
In the project directory, you can run the following scripts using pnpm:
pnpm run dev:
Runs the app in development mode with hot reloading.
Open http://localhost:5173 to view it in the browser.
pnpm run build:
Builds the app for production to the dist folder.
It correctly bundles React in production mode and optimizes the build for the best performance.
pnpm run lint:
Lints the project files using ESLint (if configured).
pnpm run preview:
Serves the production build from the dist folder locally. This is a good way to test the production build before deploying.
Project Structure
public/: Contains static assets.
src/: Contains the main application source code.
components/: React components for different sections of the website.
lib/: Contains the core JavaScript logic for Markov Chains (markov_logic.js) and the interactive visualization (interactive_visualization_logic.js).
App.jsx: The main application component that structures the pages.
main.jsx: The entry point for the React application.
index.css: Global styles and Tailwind CSS imports.
index.html: The main HTML file.
package.json: Defines project metadata, dependencies, and scripts.
pnpm-lock.yaml: Records the exact versions of dependencies.
vite.config.ts: Configuration file for Vite.
tailwind.config.js: Configuration file for Tailwind CSS.
