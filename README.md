<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title contenteditable="false">My Homepage — editable</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="container">
    <header class="hero">
      <div class="hero-left">
        <h1 id="name" class="editable" data-key="name" data-default="Your Name" contenteditable="true">Your Name</h1>
        <p id="subtitle" class="editable muted" data-key="subtitle" data-default="One-sentence summary about you — edit me!" contenteditable="true">One-sentence summary about you — edit me!</p>
        <div class="controls">
          <button id="saveBtn">Save</button>
          <button id="resetBtn">Reset</button>
          <button id="exportBtn">Export JSON</button>
          <button id="importToggleBtn">Import JSON</button>
        </div>
      </div>
      <div class="hero-right">
        <img src="https://placehold.co/160x160?text=Avatar" alt="avatar" class="avatar" />
      </div>
    </header>

    <main>
      <section>
        <h2>About</h2>
        <div id="bio" class="editable" data-key="bio" data-default="Write a short bio about yourself here. What do you do? What are you passionate about?" contenteditable="true">
          Write a short bio about yourself here. What do you do? What are you passionate about?
        </div>
      </section>

      <section>
        <h2>Skills</h2>
        <ul id="skills" class="editable-list" data-key="skills" data-default='["HTML","CSS","JavaScript"]'>
          <li contenteditable="true">HTML</li>
          <li contenteditable="true">CSS</li>
          <li contenteditable="true">JavaScript</li>
        </ul>
        <button id="addSkillBtn" class="small">+ Add skill</button>
      </section>

      <section>
        <h2>Projects</h2>
        <div id="projects" class="editable" data-key="projects" data-default='<ul><li contenteditable="true">Project A — short description</li><li contenteditable="true">Project B — short description</li></ul>' contenteditable="true">
          <ul>
            <li contenteditable="true">Project A — short description</li>
            <li contenteditable="true">Project B — short description</li>
          </ul>
        </div>
      </section>

      <section>
        <h2>Contact</h2>
        <div id="contact" class="editable" data-key="contact" data-default="Email: you@example.com — Twitter: @you" contenteditable="true">
          Email: you@example.com — Twitter: @you
        </div>
      </section>
    </main>

    <footer>
      <small>&copy; <span id="year"></span> <span id="footerName" data-key="footerName" data-default="Your Name" contenteditable="true">Your Name</span></small>
    </footer>

    <div id="importArea" class="import-area hidden">
      <textarea id="importTextarea" placeholder='Paste exported JSON here'></textarea>
      <div class="import-controls">
        <button id="importBtn">Import</button>
        <button id="cancelImportBtn">Cancel</button>
      </div>
    </div>
  </div>

  <script src="script.js"></script>
</body>
</html>
