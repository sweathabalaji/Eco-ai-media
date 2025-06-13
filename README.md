# Eco-ai-media
## Objective

Design and develop a responsive single-page portfolio website with modern frontend technologies and mandatory 3D model integration to demonstrate clean, interactive, and visually appealing web development skills with a solid code structure.

## Task Breakdown

### 1. Portfolio Website (Frontend)

Develop a single-page responsive portfolio website using one of the following tech stacks:

- **HTML, CSS, JavaScript** (Vanilla or React)
- **Frameworks Allowed**: Tailwind CSS, Bootstrap

### Website Sections

The website must include the following sections:

**A. Hero Section**

- **Content**:
    - Full name
    - Role (e.g., Web Developer, Designer, etc.)
    - Background image
    - Optional: Call-to-action button (e.g., "View My Work")
- **Purpose**: Create an engaging first impression with a professional layout and visually appealing background.

**B. About Section**

- **Content**:
    - Short introduction paragraph about yourself (e.g., background, skills, passion)
    - Profile picture
- **Purpose**: Provide a personal touch and context about your expertise.

**C. Projects Section**

- **Content**:
    - Showcase 2–3 sample or dummy projects
    - Each project must include:
        - Project title
        - Preview image or screenshot
        - Short description
        - Link (e.g., GitHub repository or placeholder URL)
- **Purpose**: Highlight your technical abilities and creativity through project examples.

**D. Contact Section**

- **Content**:
    - Simple contact form with fields:
        - Name
        - Email
        - Message
    - JavaScript validation to check:
        - Empty fields
        - Valid email format (e.g., using regex: `^[^\s@]+@[^\s@]+\.[^\s@]+$`)
- **Purpose**: Allow visitors to reach out with a functional and validated form.

### Technical Requirements

- **Responsiveness**: Ensure the website is fully responsive for mobile and desktop devices using techniques like CSS media queries or framework utilities (e.g., Tailwind CSS responsive classes).
- **Folder Structure**:
    
    ```
    /portfolio
    ├── /css
    │   └── styles.css
    ├── /js
    │   └── script.js
    ├── /images
    │   ├── background.jpg
    │   ├── profile.jpg
    │   ├── project1.jpg
    │   ├── project2.jpg
    │   └── project3.jpg
    ├── /components
    │   ├── hero.html
    │   ├── about.html
    │   ├── projects.html
    │   └── contact.html
    └── index.html
    
    ```
    
- **Code Quality**:
    - Include meaningful comments in HTML, CSS, and JavaScript files.
    - Write readable and maintainable code (e.g., consistent naming, modular structure).
- **Bonus**: Deploy the website on GitHub Pages, Vercel, or Netlify and provide the live link.

### 2. 3D Model Integration (Mandatory)

Integrate a 3D model or scene into the Hero or Projects section using one of the following methods:

### Option A: Three.js

- **Task**:
    - Import and render a basic interactive 3D model (e.g., spinning cube, 3D icon, or glTF file).
    - Enable basic interactions (e.g., rotation, zoom).
- **Implementation Steps**:
    1. Include Three.js via CDN: `<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>`.
    2. Create a canvas element in the chosen section (Hero or Projects).
    3. Write JavaScript to:
        - Initialize a scene, camera, and renderer.
        - Load a 3D model (e.g., glTF using `GLTFLoader`) or create a simple geometry (e.g., cube).
        - Add OrbitControls for rotation and zoom.
        - Animate the model (e.g., auto-rotation).
    4. Style the canvas to fit responsively within the section.
- **Integration**: Embed the 3D model in the Hero section as a background element or in the Projects section as a project showcase.

### Option B: Spline

- **Task**:
    - Create or use a pre-built 3D scene from [Spline](https://spline.design/).
    - Embed the scene using an iframe or export code provided by Spline.
- **Implementation Steps**:
    1. Design a simple 3D scene in Spline (e.g., animated icon or abstract shape).
    2. Export the scene as an iframe or JavaScript embed code.
    3. Integrate the iframe/code into the Hero or Projects section.
    4. Ensure the embedded scene is responsive and styled to match the website’s design.
- **Integration**: Use in the Hero section for visual impact or in the Projects section to enhance a project’s presentation.

### Notes

- Choose the integration method based on your familiarity with Three.js or Spline.
- Ensure the 3D element enhances the section’s purpose without overwhelming the design.
- Test interactions (e.g., rotation, zoom) on both desktop and mobile devices.

### 3. Optional (Bonus): WordPress / Node.js Integration

Describe how you would implement 3D integration in the following environments:

### WordPress

- **Methods**:
    - **Plugin-Based Embedding**: Use a plugin like "Insert HTML Snippet" or "Embed Any Document" to add Three.js or Spline embed code.
    - **Custom Theme Development**: Create a custom WordPress theme and add the 3D model code directly in the theme’s template files (e.g., `front-page.php`).
    - **Iframe Usage**: Embed the Spline scene via an iframe in a page or post using the WordPress editor or a shortcode.
- **Steps**:
    1. Install WordPress locally or on a hosting service.
    2. For Three.js:
        - Add Three.js CDN and custom JavaScript to the theme’s `functions.php` or a custom plugin.
        - Create a shortcode to render the 3D model in the desired section.
    3. For Spline:
        - Copy the iframe code from Spline.
        - Paste it into a WordPress page or post using the block editor or a shortcode.
    4. Ensure responsiveness using CSS in the theme’s stylesheet.

### Node.js

- **Methods**:
    - **Three.js with Express**: Serve a static HTML page with Three.js integration using Express.
    - **React-Based Frontend**: Integrate Three.js or Spline in a React component for a dynamic frontend.
- **Steps**:
    1. **Three.js with Express**:
        - Set up an Express server with a route to serve `index.html`.
        - Include Three.js and the 3D model code in the HTML file.
        - Use a static folder for assets (`/images`, `/js`).
    2. **React-Based Frontend**:
        - Create a React app using `create-react-app`.
        - Install `@react-three/fiber` and `@react-three/drei` for Three.js integration.
        - Build a component to render the 3D model.
        - For Spline, use the `@splinetool/react-spline` package or an iframe.
    3. Ensure the server or frontend is responsive and optimized for performance.

## Deliverables

1. **Source Code**:
    - Provide a GitHub repository or zipped project folder with the complete codebase.
    - Ensure the folder structure is clean and includes all assets (images, scripts, styles).
2. **Deployment Link**:
    - Deploy the website on GitHub Pages, Vercel, or Netlify.
    - Share the live URL in the documentation.
3. **Documentation**:
    - Create a `README.md` file including:
        - Tools and technologies used (e.g., HTML, Tailwind CSS, Three.js).
        - Deployment steps (e.g., `npm install`, `vercel deploy`).
        - 3D integration method (Three.js or Spline) and where it’s implemented.
        - Any setup instructions or dependencies.
    - Example `README.md` structure:
        
        ```
        # Portfolio Website
        ## Overview
        A responsive single-page portfolio website built for the Web Development Internship Assignment.
        ## Technologies Used
        - HTML, CSS, JavaScript
        - Tailwind CSS
        - Three.js (for 3D model integration)
        ## Deployment
        - Deployed on: [Vercel URL]
        - Steps: `npm install`, `vercel deploy`
        ## 3D Integration
        - Method: Three.js
        - Location: Hero section
        - Description: Spinning 3D cube with OrbitControls for rotation and zoom.
        ## Setup Instructions
        1. Clone the repository: `git clone [repo-url]`
        2. Open `index.html` in a browser or deploy to a hosting platform.
        
        ```
        
4. **Optional: Walkthrough**:
    - Record a 1–2 minute Loom or screen-recorded video demonstrating:
        - Navigation through the website sections.
        - Interaction with the 3D model (e.g., rotation, zoom).
        - Form validation functionality.
        - Responsiveness on mobile and desktop views.

## General Guidelines

- **Responsiveness**: Test the website on multiple devices (e.g., Chrome DevTools responsive mode) to ensure compatibility.
- **Code Quality**:
    - Use consistent indentation (2 or 4 spaces).
    - Add comments to explain key sections of code (e.g., 3D model initialization, form validation logic).
    - Modularize code where possible (e.g., separate JavaScript functions for form validation and 3D rendering).
- **Performance**:
    - Optimize images (e.g., compress using tools like TinyPNG).
    - Minimize external dependencies to reduce load times.
- **Accessibility**:
    - Use semantic HTML (e.g., `<section>`, `<header>`, `<footer>`).
    - Add `alt` attributes to images.
    - Ensure keyboard navigation for interactive elements (e.g., form, 3D model controls).
- **Bonus**: A live deployment showcases your ability to deliver a production-ready website.
