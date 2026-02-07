<h1 align="center">💬 Web Chat Application</h1>
<p align="center">A real-time web chat application built with Django, Redis, and Docker.</p>
<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
</p>
<hr />

<h2>📦 Project Setup</h2>
<p>You can run this Web Chat Application in <strong>two different ways</strong>:</p>

<ul>
  <li><strong>Method 1:</strong> Using Docker 🐳</li>
  <li><strong>Method 2:</strong> Running directly on your system ⚙️</li>
</ul>

<hr />

<h2>🐳 Method 1: Run Using Docker</h2>
<h3>Option A: Use Prebuilt Docker Image (Recommended)</h3>
<p>You can also run the application using a prebuilt private Docker image hosted on <strong>GitHub Container Registry (GHCR)</strong>.</p>

<ol><li>Pull the Docker image:</li></ol>
<pre><code>docker pull ghcr.io/sagar-ph/webapp:latest</code></pre>
<ol start="2"><li>Get the <code>docker-compose.yml</code> file in repo and Update the file:</li></ol>
<pre><code>image: ghcr.io/sagar-ph/webapp:latest</code></pre>
<p><strong>Note:</strong> Remove or comment out <code>build: .</code> if present.</p>
<ol start="3"><li>Start the application:</li></ol>

<pre><code>docker compose up</code></pre>
<p>This will pull and run all required services in Docker containers.</p>

<hr />

<h3>🚀 Clone the Repository (For below Methods)</h3>
<pre><code>gh repo clone Sagar-PH/WebChat-App</code></pre>

<hr />

<h3>Option B: Build Docker Image Locally</h3>

<ol>
  <li>Make sure <strong>Docker</strong> is installed on your system.</li>
  <li>Open a terminal in the project directory.</li>
  <li>Build the Docker image:</li>
</ol>

<pre><code>docker build -t webchat-app .</code></pre>
<p>This command will build and create a Docker image for the project.</p>

<hr />

<h2>⚙️ Method 2: Run Directly (Without Docker)</h2>
<h3>Prerequisites</h3>
<ul>
  <li>Python 3.x</li>
  <li>Redis Server</li>
</ul>

<h3>Steps</h3>
<ol>
  <li>Install and start the Redis server.</li>
  <li>Open a terminal in the project directory.</li>
  <li>Install project dependencies:</li>
</ol>

<pre><code>pip install -r requirements.txt</code></pre>
<ol start="4"><li>Run the Django ASGI application:</li></ol>
<pre><code>daphne webchat.asgi:application</code></pre>
<p>🎉 The Web Chat Application is now running!</p>

<hr />

<p align="center">Made by <strong>Sagar</strong></p>

<hr />

<h2>Project Demo</h2>
<img src="https://sagar-ph.github.io/Images/Chat-Project.png">
