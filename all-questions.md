# Development interview questons

1.  **_What happens in the browser when we open a HTML file in it ?_**
    <details>
    <summary>Answer</summary>

    - When we feed HTML file in the browser lot of steps happen. These steps are called as CRP (Critical Rendering Path).
        1. Construction of DOM tree.
        2. Construction of CSSOM tree.
        3. Running Javascript
        4. Creation of the Render tree.
        5. Layout
        6. Painting.

    - **_Step 1:_** Construction of DOM tree.
        - In computers there are lots of situation where the computer need to store hierarchy based data.
        - Tree is a way to store hierarcy based data.
        - The tree which stores the HTML data is called as **DOM Tree**. DOM tree stores the hierarchy based structure of HTML.
    
    - **_Step 2:_** Construction of CSSOM tree.
        - Just like DOM is created for HTML, CSSOM is created for CSS.
    
    - **_Step 3:_** Running the Javascript.
    
    - **_Step 4:_** Construction of Render tree.
        - After the above 3 steps one new tree is form called as ***Render Tree***.
        - Render tree is a combination of ***DOM*** and ***CSSOM***. It only contain visible elements of the page.
    
    - **_Step 5:_** Layout.
        - Also called as ***reflow***.
        - This step does all the measurement, also calculate position on the page where elements are placed.
    
    - **_Step 6:_** Painting.
        - At this step page is painted pixel by pixel on screen.
    

    ![alt text](https://web.dev/static/articles/critical-rendering-path/render-tree-construction/image/dom-cssom-are-combined-8de5805b2061e.png)

    </details>