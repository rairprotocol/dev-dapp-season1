---
title: Untitled

---

# GitHub Task: Vibe-Code and Deploy a Game or App with Astro and Netlify

## Objective
In this exciting task, you’ll unleash your creativity to vibe-code a **game or web app** of your choice using the Astro Wind template, deploy it to Netlify, and share your masterpiece by submitting an issue to a designated GitHub repository. Whether you’re crafting a simple puzzle game, a to-do list app, or something totally unique, this task is your chance to build something cool, deploy it to the open internet for free, and show it off to the world!

## Why This Is Awesome
You don’t need to be a coding expert to make something amazing. With Astro Wind’s open-source template, Cursor’s AI-powered coding assistance, and Netlify’s seamless deployment, you’ll go from zero to a live app in no time. This task is all about experimenting, having fun, and learning how to ship a project end-to-end. Let’s get started and create something you’re proud to share!

## Prerequisites
Before diving in, make sure you have:
- A GitHub account (free at [github.com](https://github.com/)).
- A Netlify account (free tier at [netlify.com](https://www.netlify.com/)).
- [Cursor IDE](https://cursor.com/) installed (grab the free trial!).
- Node.js and npm installed ([nodejs.org](https://nodejs.org/)).
- Git installed ([git-scm.com](https://git-scm.com/)).

## Task Instructions
Follow these steps to vibe-code your game or app, deploy it, and submit it for credit. Each step is designed to guide you through the process while giving you room to explore your ideas.

1. **Create Your GitHub Repository**
   - Head to the [Astro Wind GitHub repository](https://github.com/onwidget/astrowind).
   - Click **Use this template** > **Create a new repository**.
   - Name your repository something fun like `my-astro-project` or `cool-game-app`.
   - Set it to **Public** so everyone can see your awesome work.
   - Create the repository to get a fresh copy of the Astro Wind template, which is like a blank canvas for your project.

2. **Deploy the Default Site to Netlify**
   - Log in to [Netlify](https://www.netlify.com/) or sign up for a free account.
   - Click **New site from Git** and connect your GitHub account.
   - Select your new repository (e.g., `my-astro-project`).
   - Use the default build settings—no changes needed yet.
   - Deploy the site. Netlify will give you a random URL (e.g., `quirky-name.netlify.app`).
   - (Optional) Go to **Site settings** > **Change site name** and pick something memorable like `my-cool-app.netlify.app`.
   - Visit your Netlify URL to confirm the default Astro Wind site is live. You’re already on the internet—how cool is that?

3. **Clone the Repository to Your Computer**
   - Open Cursor IDE (your AI coding buddy).
   - Choose **Clone Repository** and grab the HTTPS URL from your GitHub repo (find it under **Code** > **HTTPS**).
   - Save the project to a folder on your computer (works on Windows, Mac, or Linux).
   - Check that the project files load in Cursor. You’re now ready to start vibe-coding!

4. **Set Up Vibe-Coding Rules**
   - Create a file called `.cursorrules` in the project root (or use Cursor’s settings for project rules).
   - Add these rules to keep the AI focused and prevent it from going wild:
     ```markdown
     - Use only the frameworks and technologies in the Astro Wind repository.
     - Stick to TypeScript for clean, reliable code.
     - Use Tailwind CSS for styling—no other CSS frameworks.
     - Only use existing Tabler icons; don’t add new ones.
     ```
   - Save the file. These rules are like guardrails to make sure your project stays smooth and compatible.

5. **Set Up the Local Environment**
   - In Cursor, open a terminal (or use your system’s terminal in the project folder).
   - Run `npm install` to grab all the project’s dependencies.
   - Run `npm run dev` to launch a local server.
   - Open `http://localhost:4321` in your browser to see the default Astro Wind site.
   - If you hit errors, check the terminal for clues. Make sure Node.js and npm are updated, or ask Cursor to troubleshoot:
     ```
     I got this error: [paste error]. Can you help me fix it?
     ```

6. **Vibe-Code Your Game or App**
   - Decide what you want to build! It could be:
     - A game (e.g., a quiz, a simple platformer, or a clicker game).
     - An app (e.g., a weather dashboard, a note-taker, or a portfolio page).
     - Anything else that sparks your interest!
   - In Cursor, start a new conversation (`+` button) to keep things fresh.
   - Write a clear prompt for a Product Requirements Document (PRD):
     ```
     Write a detailed PRD for a [describe your idea, e.g., simple quiz game, to-do list app]. Ensure it’s on a new page (e.g., /my-app) and doesn’t break the Astro Wind site’s other features. Include a step-by-step plan for implementation.
     ```
   - Review the PRD to make sure it captures your vision (e.g., key features, page structure).
   - In a new conversation, prompt Cursor to build it:
     ```
     Implement the [game/app] from the PRD efficiently. Create a new Astro file at /src/pages/my-app/index.astro and any needed components. Make sure it’s accessible at /my-app and works with the rest of the site.
     ```
   - Accept Cursor’s changes (e.g., new files, components). If it suggests new dependencies (like React or a library for your idea), run `npm install` again.

7. **Test Your Creation Locally**
   - Run `npm run dev` to restart the local server.
   - Visit `http://localhost:4321/my-app` to see your game or app in action.
   - If it doesn’t work, don’t panic! Start a new conversation in Cursor and share the error:
     ```
     My app at /my-app failed with this error: [paste error]. Please check the /my-app folder and fix it.
     ```
   - Keep tweaking until it loads locally, even if it’s a basic version. A working prototype is something to celebrate!

8. **Push Your Changes to GitHub**
   - In Cursor, ask the AI to commit your work:
     ```
     Commit all changes to the main branch of my remote repository.
     ```
   - Or use the terminal:
     ```bash
     git add .
     git commit -m "Add my game/app"
     git push origin main
     ```
   - Check your GitHub repo to confirm the changes are there. Regular commits save your progress, so don’t skip this!

9. **Check Your Live Deployment on Netlify**
   - Visit your Netlify dashboard and look at the **Deploys** tab.
   - Ensure Netlify picks up your latest commits and builds the updated site.
   - Once the build finishes, go to `your-site-name.netlify.app/my-app` to see your game or app live.
   - If the build fails, grab the error logs from Netlify, paste them into Cursor, and ask:
     ```
     Netlify failed with this error: [paste error]. How can I fix it?
     ```
   - Recommit and redeploy until it’s live and working. You’re so close to sharing your project with the world!

10. **Submit Your Work as a GitHub Issue**
    - Go to the designated GitHub repository for submissions (provided by your instructor, e.g., a `DevDapp` repo).
    - Click **Issues** > **New issue**.
    - Fill out this template to showcase your work:
      ```markdown
      **Title**: Astro App Submission - [Your GitHub Username]

      **Description**:
      I vibe-coded a [game/app, e.g., quiz game, to-do list app] using Astro Wind and deployed it to Netlify!

      - **Netlify Deployment URL**: [e.g., https://my-cool-app.netlify.app/my-app]
      - **GitHub Repository**: [e.g., https://github.com/your-username/my-astro-project]
      - **What I Built**: [Briefly describe, e.g., "A simple quiz game where users answer trivia questions."]
      - **Notes**: [Anything else, e.g., "It’s a prototype, but I’m excited to improve it!"]

      Thanks for checking out my project!
      ```
    - Submit the issue. Make sure your Netlify URL and GitHub repo are public so your instructor can see your awesome creation.

## Deliverables
- A public GitHub repository (e.g., `my-astro-project`) with your Astro Wind project and custom game or app.
- A live Netlify deployment with your game or app accessible at `/my-app` (e.g., `your-site-name.netlify.app/my-app`).
- A GitHub issue in the designated repository with links to your Netlify site and GitHub repo, plus a description of what you built.

## Tips to Shine
- **Dream Big, Start Small**: Your game or app doesn’t need to be complex. A working prototype (like a basic game or functional app) is a huge win!
- **Save Often**: Commit to GitHub after every working change to protect your progress.
- **Test Locally**: Always check `localhost` before pushing to catch issues early.
- **Ask Cursor for Help**: If you’re stuck, use Cursor to debug errors or brainstorm ideas:
  ```
  I want to add [feature, e.g., a scoreboard]. Can you suggest how to do it in Astro?
  ```
- **Make It Yours**: Add a personal touch with Tailwind CSS styles or fun features to stand out.
- **Submit with Pride**: Even a simple project shows your effort, so share it confidently!

## How You’ll Be Evaluated
Your submission will be judged on:
- **Functionality**: Your game or app loads at `/my-app` without breaking the Astro Wind site.
- **Deployment**: The Netlify URL works and matches your submission.
- **Repository**: Your public GitHub repo includes all files and shows your commits.
- **Issue Quality**: The issue is clear, with working links and a description of your project.
- **Creativity**: Bonus points for unique ideas or extra effort, but a working project is the main goal.

## Resources to Inspire You
- [Astro Wind GitHub](https://github.com/onwidget/astrowind) - Your starting point.
- [Netlify Docs](https://docs.netlify.com/) - For deployment tips.
- [Cursor Docs](https://docs.cursor.com/) - To master vibe-coding.
- [Tailwind CSS Docs](https://tailwindcss.com/docs) - For styling your app.
- [GitHub Docs](https://docs.github.com/) - For Git basics.
- [Three.js Docs](https://threejs.org/docs/) - If you’re making a game with 3D elements.

## You’ve Got This!
This task is your playground to experiment and create something unique. Whether it’s a game that makes people smile or an app that solves a small problem, you’re learning skills that open doors in tech. Have fun vibe-coding, don’t stress about perfection, and share your project with pride. We can’t wait to see what you build!

Happy coding, and let’s make the internet a little more awesome together!

### Notes on Changes
- **Generic Focus**: Replaced the missile defense game with a flexible "game or app" to encourage creativity (e.g., quizzes, dashboards, or portfolios).
- **Encouraging Tone**: Used motivational language like “unleash your creativity,” “you’ve got this,” and “make something cool” to inspire confidence.
- **Simplified Steps**: Kept the 10-step structure but made instructions more concise and beginner-friendly, emphasizing experimentation.
- **Creative Freedom**: Prompt examples allow students to define their project while maintaining the Astro/Netlify flow.
- **Retained Core Workflow**: Followed the transcript’s process (GitHub setup, Netlify deployment, Cursor rules, local testing, iterative fixes, issue submission).
- **Evaluation Clarity**: Highlighted that a working prototype is enough, with bonus points for creativity, to reduce pressure.
- **Resources**: Included general resources (e.g., Tailwind, Three.js) to support diverse project ideas.

This version balances structure with flexibility, encouraging students to explore while ensuring they can complete the task successfully. Let me know if you’d like further tweaks!

## Labels
Label Awarded: "Vibe Dapp"
Sponsor: None
