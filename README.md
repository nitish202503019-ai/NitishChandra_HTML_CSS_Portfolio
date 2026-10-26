# NitishChandra_HTML_CSS_Portfolio
My HTML &amp; CSS Internship Portfolio
HERE IS THE CODE OF THAT 
/* Global Styles & Variables */
:root {
    --primary-color: #0056b3;
    --secondary-color: #f4f6f9;
    --text-color: #333333;
    --white: #ffffff;
    --transition: all 0.3s ease;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    color: var(--text-color);
    line-height: 1.6;
    background-color: var(--secondary-color);
}

/* Header & Navigation */
header {
    background: var(--white);
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo {
    font-weight: bold;
    font-size: 1.2rem;
    color: var(--primary-color);
}

nav ul {
    display: flex;
    list-style: none;
    gap: 20px;
}

nav a {
    text-decoration: none;
    color: var(--text-color);
    font-weight: 600;
    transition: var(--transition);
}

nav a:hover {
    color: var(--primary-color);
}

/* Sections General Styling */
section {
    padding: 4rem 10%;
    background: var(--white);
    margin-bottom: 1rem;
}

section h2 {
    text-align: center;
    margin-bottom: 2rem;
    color: var(--primary-color);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, #0056b3, #008080);
    color: var(--white);
    text-align: center;
    padding: 6rem 10%;
}

.hero h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.hero p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.btn {
    display: inline-block;
    background: var(--white);
    color: var(--primary-color);
    padding: 0.75rem 1.5rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: var(--transition);
}

.btn:hover {
    background: #e2e6ea;
}

/* Skills Section */
.skills-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
}

.skill-chip {
    background: var(--secondary-color);
    color: var(--primary-color);
    padding: 0.5rem 1.2rem;
    border-radius: 20px;
    font-weight: 600;
    border: 1px solid #d1d5db;
}

/* Projects Section */
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
}

.project-card {
    background: var(--secondary-color);
    padding: 1.5rem;
    border-radius: 8px;
    border: 1px solid #e5e7eb;
    transition: var(--transition);
}

.project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.project-card h3 {
    margin-bottom: 0.5rem;
    color: var(--primary-color);
}

.tech-used {
    display: inline-block;
    margin-top: 1rem;
    font-size: 0.85rem;
    font-weight: bold;
    color: #555;
}

/* Contact Section */
.contact {
    text-align: center;
}

.contact p {
    margin: 0.5rem 0;
}

.form-note {
    font-size: 0.85rem;
    color: #777;
    margin-top: 1rem;
}

/* Footer */
footer {
    text-align: center;
    padding: 1.5rem;
    background: #222;
    color: var(--white);
    font-size: 0.9rem;
}

/* Responsive Media Query for Smaller Screens */
@media (max-width: 768px) {
    header {
        flex-direction: column;
        gap: 10px;
    }

    nav ul {
        gap: 10px;
        flex-wrap: wrap;
        justify-content: center;
    }

    .hero h1 {
        font-size: 2rem;
    }
    
    section {
        padding: 3rem 5%;
    }
