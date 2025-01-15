# HTML - Curiculum "Websites for beginners"
## Class 1
- Introduction
    + How the web works
        - Sites, Servers, Browsers 
        - TCP/IP, DNS
- Setting up your Environment - IDE
    + VS Code - Visual Studio Code
    + Notepad++
    + Notepad
- HTML Basics
    + HTML
        - .html, .htm
        - Elements - Tags
        - CSS - Cascading Style Sheets - .css
        - Javascript - .js
    + First Site - Jello World
        - Use Notepad
        - Create File - first.html
        - Inside first.html
        <html>
            Jello World!
        </html>
- Homework
    + What does TCP/IP stand for?
    + What does DNS stand for?
## Class 2
- HTML Elements - Tags
    + HTML - Cosists of elements called tags
    + Tags must be closed </>
    + There are many tags
    + h - Heading
    ```
    <h>h</>
    ```
    + p - Paragrph
    ```
    <p>some text or content</p>

    ```
    + a - Anchor or hyperlink or link
    ```
    <a href="http://example.com">This is the text that is displayed</a>

    ```
    + img - Image, picture
    ```
    <img src="yourImage.jpg" alt="alternative text for text readers">

    ```
    + div - Division
    ```
    <div></div>

    ```
- Second Site - Two pages with navigation
    + Use VS Code
- Homework
    + What does HTML stand for?
## Class 3
- Bash
    + Command Line - CLI
    + bash - just go ahead and stick your nose in the air :)
    + Git - VCS - Version Control Software
        - github.com
        - Repositories - Repos
        - basic commands in bash - terminal
        ```
        git add .
        git commit -m"describes the work you are saving"
        git push
        ```
- VS Code
- Github.com
    + Create account on github.com
    + Create Repo
    + Clone the repo
    + Open VS Code and start a terminal - bash
    + Copy the git reference
    ```
    git clone <paste in the text from github>
    ```
- Best Practices
    + Commit when you have completed work
    + Commit often - 2-3 times per hour
## Class 4
- CSS - Cascading Style sheets
    + CSS makes the html more visialy appealing
    + Allows you to create your own layout, or how the page is arranged
    + Along with HTML, CSS forms the basis of a web page
    + Three ways to use CSS
        - Under the style element in head
        ```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Mark King - Portfolio</title>
            <style>
                .someClass{
                    background-color:"blue";
                }
            </style>
        </head>
        <body>
            <p class="someClass">Some Content</p>
        </body>
        </html>
        ```
        - with a linked style sheet saved with a .css extension
        ```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Mark King - Portfolio</title>
            <link rel="stylesheet" href="styles.css">
        </head>
        <body>
            <p class="someClass">Some Content</p>
        </body>
        </html>
        ```
        - Inline
        ```
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Mark King - Portfolio</title>
        </head>
        <body>
            <p style="background-color:blue;">Some Content</p>
        </body>
        </html>    

        ```
## Class 5 - CSS Layout
- Many types of Layout Techniques
    - Fixed
    - Flexbox
    - Frameworks
    - Grid - What we are going to use
- Grid
    + HTML
    ```
    <html>
    <body>
        <div class="wrapper">
            <div class="logo">logo</div>
            <div class="header">header</div>
            <div class="nav">nav</div>
            <div class="content">content
                <p>Lorem ipsum dolor.</p>
            </div>
            <div class="footer">Footer</div>
        </div>
    </body>
    </html>
    ```
    + CSS
    ```
    .wrapper {
        display: grid;
        grid-template-columns: repeat(5,1fr);
        grid-template-rows: repeat(5,1fr);
        grid-template-areas: 
            "a b b b c"
            "d e e e f"
            "d e e e f"
            "d e e e f"
            "d g g g f";
    }
    .logo {
        grid-area: a;
    }
    .header {
        grid-area: b;
    }
    .nav {
        grid-area: c;
    }
    .content {
        grid-area: e;
    }
    .footer {
        grid-area: g;
    }

    ```
## Class 6 - Review and Certification
- Certificatin Site
    + New github repo
    + Single page site
- Practice 3 page layout site