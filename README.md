# MDAP-EX_01-Portfolio
## Date: 10/08/2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Harini Anand - Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navigation -->
    <header>
        <nav>
            <h1 class="logo">Harini Anand</h1>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#skills">Skills</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="home-section">
        <div class="about-text">
            <h2>Hello, I'm Harini 👋</h2>
            <p>
                I'm a pre-final year Computer Science student at Saveetha Engineering College.  
                I’m passionate about web development and design — I love creating visually appealing,  
                functional websites and crafting smooth user experiences.
            </p>
        </div>
        <div class="profile-pic">
            <img src="images/me.jpg" alt="Harini Profile">
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects-section">
        <h2>My Projects</h2>
        <div class="projects-grid">
            <div class="project-card dark-pink">
                <h3>SKYN</h3>
                <p>A skincare brand e-commerce platform built with HTML & CSS,  
                focusing on minimal, clean, and modern design.</p>
            </div>
            <div class="project-card medium-pink">
                <h3>Ghost Fishing</h3>
                <p>An IoT-based solution for detecting and reducing ghost fishing,  
                helping marine conservation efforts.</p>
            </div>
            <div class="project-card light-pink">
                <h3>AI Mood Journal</h3>
                <p>An AI-powered journal that analyzes user entries to understand  
                mood patterns and provide personalized insights.</p>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills-section">
        <h2>My Skills</h2>
        <div class="skill">
            <p>Python</p>
            <div class="bar"><div class="fill python"></div></div>
        </div>
        <div class="skill">
            <p>C</p>
            <div class="bar"><div class="fill c"></div></div>
        </div>
        <div class="skill">
            <p>HTML</p>
            <div class="bar"><div class="fill html"></div></div>
        </div>
        <div class="skill">
            <p>CSS</p>
            <div class="bar"><div class="fill css"></div></div>
        </div>
        <div class="skill">
            <p>JavaScript</p>
            <div class="bar"><div class="fill js"></div></div>
        </div>
        <div class="skill">
            <p>React</p>
            <div class="bar"><div class="fill react"></div></div>
        </div>
    </section>

</body>
</html>
```
style.css
```
/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background-color: #191516;
    background-image: url("https://www.transparenttextures.com/patterns/asfalt-light.png");
    background-repeat: repeat;
    color: #FFD9DA;
    line-height: 1.6;
}

/* Navigation */
header {
    background: #382E31;
    padding: 15px 30px;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 10;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav .logo {
    font-size: 1.5em;
    color: #FFD9DA;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 20px;
}

nav ul li a {
    color: #FFD9DA;
    text-decoration: none;
    font-weight: bold;
}

nav ul li a:hover {
    color: #EB638B;
}

/* Home Section */
.home-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 100px 30px;
    min-height: 100vh;
}

.about-text {
    width: 50%;
}

.profile-pic {
    width: 300px;
    height: 300px;
    border-radius: 50%;
    background-color: #FFD9DA;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    box-shadow: 0 0 20px rgba(255, 217, 218, 0.5);
}

.profile-pic img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Projects Section */
.projects-section {
    padding: 100px 30px;
    text-align: center;
}

.projects-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    margin-top: 30px;
}

.project-card {
    padding: 20px;
    border-radius: 10px;
    color: #fff;
    min-height: 150px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(255, 217, 218, 0.3);
}

.dark-pink {
    background-color: #AC274F;
}

.medium-pink {
    background-color: #EB638B;
}

.light-pink {
    background-color: #FFD9DA;
    color: #191516;
    grid-column: span 2;
}

/* Skills Section */
.skills-section {
    padding: 100px 30px;
}

.skill {
    margin-bottom: 20px;
}

.bar {
    background: #382E31;
    border-radius: 5px;
    overflow: hidden;
    height: 20px;
}

.fill {
    height: 100%;
    text-align: right;
    padding-right: 5px;
    color: white;
    font-size: 12px;
}

.python { width: 85%; background: #EB638B; }
.c { width: 80%; background: #AC274F; }
.html { width: 95%; background: #FFD9DA; color: #191516; }
.css { width: 90%; background: #EB638B; }
.js { width: 85%; background: #AC274F; }
.react { width: 75%; background: #382E31; }
```

## OUTPUT

![WhatsApp Image 2025-08-11 at 10 48 50_e98e6767](https://github.com/user-attachments/assets/731212ab-6419-45e4-868f-af3b6cd8e4dc)

![WhatsApp Image 2025-08-11 at 10 49 14_9afe0c62](https://github.com/user-attachments/assets/f7410566-57f6-433e-9c5b-c681385cf1f5)

![WhatsApp Image 2025-08-11 at 10 49 35_c85150f6](https://github.com/user-attachments/assets/228b1a0c-e496-4133-a52c-b3b141db86eb)


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
