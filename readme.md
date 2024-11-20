# Web Development Cheatsheet

---

## 1.1 How the Web Works
- **Key Concepts**:
  - **Client-Server Model**:  
    - **Client**: Browser sends a request (HTTP/HTTPS).  
    - **Server**: Returns a response (HTML, CSS, JavaScript, or other data).
  - **HTTP/HTTPS**: Protocols used for communication between clients and servers.
  - **DNS (Domain Name System)**: Resolves human-readable domain names to IP addresses.
  - **Rendering**: Browser interprets received files to display a webpage.

- **Lifecycle of a Web Request**:
  1. Enter URL in browser.
  2. Browser queries DNS to get server IP.
  3. Sends an HTTP/HTTPS request to the server.
  4. Server responds with resources (HTML, CSS, JS).
  5. Browser renders and displays the page.

---

## 1.2 The HTML, CSS, and JavaScript Triangle
- **HTML (Hypertext Markup Language)**:  
  - Structure and content of the webpage (e.g., headings, paragraphs, links).
  - Example:  
    ```html
    <h1>Hello, World!</h1>
    ```

- **CSS (Cascading Style Sheets)**:  
  - Styles and layout (e.g., colors, fonts, positioning).
  - Example:  
    ```css
    h1 {
      color: blue;
      font-size: 24px;
    }
    ```

- **JavaScript (JS)**:  
  - Interactivity and behavior (e.g., animations, user input handling).
  - Example:  
    ```javascript
    document.querySelector('h1').textContent = 'Welcome!';
    ```

- **Relationship**:
  - **HTML** provides structure.
  - **CSS** styles the structure.
  - **JavaScript** makes it dynamic.

---

## 1.3 The Web Standards Model
- **Core Principles**:
  - Separation of Concerns:
    - **HTML**: Content.
    - **CSS**: Presentation.
    - **JavaScript**: Behavior.
  - **Accessibility**: Ensure content is accessible to all users, including those with disabilities.
  - **Cross-Browser Compatibility**: Adhere to web standards to ensure consistent rendering.

- **Layers**:
  1. **Content Layer**: HTML.
  2. **Presentation Layer**: CSS.
  3. **Behavior Layer**: JavaScript.

---

## 1.4 How Browsers Load Webpages
- **Steps in Loading**:
  1. **Parse HTML**: Construct the **DOM Tree** (Document Object Model).
  2. **Fetch Resources**: CSS, JavaScript, images, and other files.
  3. **Parse CSS**: Build the **CSSOM Tree** (CSS Object Model).
  4. **Combine DOM & CSSOM**: Create the **Render Tree**.
  5. **Layout**: Determine element positions and sizes.
  6. **Painting**: Draw elements to the screen.
  7. **JavaScript Execution**:
     - JS execution may modify the DOM, causing reflows or repaints.

- **Optimization**:
  - Use **defer** or **async** for JS to avoid blocking rendering.
  - Minimize CSS and JS files to reduce load times.
  - Utilize caching and CDNs.

---
