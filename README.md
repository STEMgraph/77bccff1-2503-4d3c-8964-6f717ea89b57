<!---
{
  "id": "77bccff1-2503-4d3c-8964-6f717ea89b57",
  "depends_on": ["3ee0acd9-0f99-4423-b4f3-a0ca84a16422"],
  "author": "Stephan Bökelmann",
  "first_used": "2025-04-13",
  "keywords": ["HTML", "semantic tags", "vim", "structure", "best practices"]
}
--->

# Structuring HTML with Semantic Tags

> In this exercise you will learn how to use semantic HTML tags such as `<article>`, `<section>`, `<nav>`, and `<footer>` to give meaningful structure to a web page. Furthermore we will explore how these tags improve clarity, maintainability, and accessibility.

### Introduction

Modern web development emphasizes not just what a page looks like, but how its structure conveys meaning. Semantic HTML tags are specially designed elements that describe their content clearly to both browsers and developers. Unlike generic `<div>` or `<span>` tags, semantic tags like `<nav>`, `<section>`, `<article>`, and `<footer>` signal the role of their content, making your markup more readable and easier to work with.

These tags are particularly useful for documentation, blogs, portfolios, and any content that benefits from logical, well-defined sections. For example, a `<nav>` tag defines a navigation menu, `<section>` defines thematic groups of content, `<article>` is suited for self-contained entries like posts or reports, and `<footer>` usually holds contact info, copyrights, or links.

Using semantic HTML also helps search engines and assistive technologies better interpret your content. It's not just best practice — it's essential for building inclusive and professional web pages.

### Further Readings and Other Sources

- [MDN Web Docs: HTML Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)
- [HTML5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
- [Accessible Web Design Principles](https://webaim.org/techniques/semanticstructure/)

---

## Tasks

### Task 1: Create a New HTML File with a Basic Structure

In this task, you'll set up a basic HTML5 document structure. This foundation will support the semantic elements you'll add in later tasks.

1. Open your terminal and create a new file with vim:
   ```sh
   vim semantic_layout.html
   ```
2. Press `i` to enter INSERT mode and begin editing the file.

3. Start with this basic HTML structure:
   ```html
   <!DOCTYPE html>
   <html>
   <head>
       <title>My Semantic Page</title>
   </head>
   <body>
   </body>
   </html>
   ```
4. Save and exit with `:wq`.

### Task 2: Add a Navigation Section

Now let’s define a navigation menu using the `<nav>` tag. This tag semantically identifies the section of the page meant for navigating between parts of the site.

1. Reopen the file and add the following inside the `<body>`:
   ```html
   <nav>
       <ul>
           <li><a href="#home">Home</a></li>
           <li><a href="#articles">Articles</a></li>
           <li><a href="#contact">Contact</a></li>
       </ul>
   </nav>
   ```
2. Save and preview your file in a browser.

### Task 3: Add Main Content Sections

Here, you’ll introduce two semantic tags: `<section>` for grouping related content and `<article>` for self-contained entries. This structure is ideal for blog posts or distinct topics.

1. Below the `<nav>`, add:
   ```html
   <section id="home">
       <h1>Welcome to My Page</h1>
       <p>This is the homepage section where we greet our visitors.</p>
   </section>

   <section id="articles">
       <article>
           <h2>First Blog Post</h2>
           <p>This article explains how semantic HTML improves structure and accessibility.</p>
       </article>

       <article>
           <h2>Second Blog Post</h2>
           <p>This entry explores best practices for organizing web content using tags.</p>
       </article>
   </section>
   ```

### Task 4: Add a Footer

Let’s add a `<footer>` to provide standard page-end content such as legal notices or author credits. This is a great place to include meta-information about the document.

1. Append the following to the bottom of `<body>`:
   ```html
   <footer>
       <p>&copy; 2025 by Your Name. All rights reserved.</p>
   </footer>
   ```
2. Save and exit vim with `:wq`.

### Task 5: Explore and Modify the Structure

Finally, experiment with what you've built. This task encourages you to interact with the layout by adding content and testing how the structure behaves in the browser.

1. Open the file in a browser to view the layout.
2. Try changing the text inside each section and adding another `<article>`.
3. Optionally add `id` attributes to each tag and link them via anchors in your `<nav>` list for quick navigation.

---

## Questions

1. What is the purpose of using a `<nav>` tag instead of a generic `<div>`?
2. How does a `<section>` differ from an `<article>` in terms of content structure?
3. What information is typically included in a `<footer>` tag?
4. Why is semantic HTML beneficial for accessibility and SEO?
5. Can multiple `<article>` tags be placed inside one `<section>`? Why or why not?

---

## Advice

As you continue building web pages, prioritize structure and clarity. Semantic tags are more than just labels — they form the blueprint of readable and maintainable HTML. They make it easier to update content, enhance accessibility for screen readers, and improve SEO. Think of each semantic tag as a signpost for both people and machines navigating your site.