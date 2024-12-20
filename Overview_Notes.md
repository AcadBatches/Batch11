# **HTML and CSS Basics: Learning Notes**

## **1. HTML Basic Syntax**

HTML (Hypertext Markup Language) is the standard language used to create web pages. It uses a series of elements represented by tags, which define the structure of the content. HTML tags typically come in pairs: an opening tag and a closing tag.

The basic structure of an HTML document includes:
- **DOCTYPE** declaration to specify the HTML version.
- **`<html>`** as the root element.
- **`<head>`** section for metadata, including title and character set.
- **`<body>`** section for the visible content on the web page.

---

## **2. Difference Between CSS and HTML**

- **HTML (Hypertext Markup Language)**: Defines the structure and content of a web page, such as headings, paragraphs, links, and images.
- **CSS (Cascading Style Sheets)**: Controls the presentation, formatting, and layout of HTML elements, such as colors, fonts, and spacing.

### **Key Differences:**
- **HTML** is about structure and content.
- **CSS** is about style and design.

---

## **3. Basics of HTML**

### **Common HTML Tags:**

- **`<img>`**: Embeds an image into the webpage. It requires the `src` attribute to define the image source.
- **`<p>`**: Defines a paragraph of text.
- **`<h1>` to `<h6>`**: Represent headings, with `<h1>` being the most important and `<h6>` the least.
- **`<a href="">`**: Defines a hyperlink. The `href` attribute specifies the URL.

---

## **4. List Formatting in HTML**

Lists are essential for organizing content. There are two types of lists in HTML:
1. **Unordered List**: Represents a list of items with no particular order (typically represented with bullets).
2. **Ordered List**: Represents a list of items in a specific order (usually with numbers).
   
### **Common Layouts Using Lists:**
- **Navigation Bar (NavBar)**: A navigation bar typically uses an unordered list to display menu items as clickable links.
- **Sidebar**: Often uses lists to display links to other pages or sections of the site.

---

## **5. Forms in HTML**

Forms are used to collect user input, such as text, selections, and submissions. Key form elements include:
- **`<input>`**: Used for various types of input fields, like text, checkboxes, radio buttons, etc.
- **`<textarea>`**: Allows users to enter multi-line text.
- **`<select>`**: Creates a dropdown list for selecting one or more options.

---

## **6. Semantics in HTML**

Semantic HTML refers to using HTML tags that convey meaning about the content they enclose. This helps with SEO (Search Engine Optimization) and accessibility. Some examples include:
- **`<header>`**: Represents the header of a section or page.
- **`<footer>`**: Defines the footer of a section or page.
- **`<article>`**: Represents a self-contained piece of content.
- **`<section>`**: Represents a thematic grouping of content.
- **`<aside>`**: Represents content that is tangentially related to the content around it, such as a sidebar.

Using semantic tags improves readability, both for developers and search engines, and ensures that content is presented logically.

---

## **7. CSS Basics**

### **CSS Selectors**
- **Element selector**: Targets all elements of a specific type.
- **Class selector**: Targets elements with a specific class.
- **ID selector**: Targets elements with a specific ID.

### **CSS Properties**
- **Color**: Defines the text color.
- **Font-family**: Specifies the font to use.
- **Margin**: Defines space around elements.
- **Padding**: Defines space inside elements.

### **Common Layouts and Styles**
- **Flexbox**: A layout model that allows easy arrangement of elements in rows or columns.
- **Grid**: A layout system that allows for complex, two-dimensional arrangements.

---

## **8. Positioning in CSS**

CSS **positioning** allows you to control the layout of elements on a webpage. There are several types of positioning:

- **Static**: Default positioning for all elements. Elements are positioned based on normal document flow.
- **Relative**: Positions an element relative to its original position.
- **Absolute**: Positions an element relative to the nearest positioned ancestor (non-static).
- **Fixed**: Positions an element relative to the viewport, meaning it stays in place when scrolling.
- **Sticky**: Combines relative and fixed positioning, allowing elements to stick to the top when scrolling past them.

### **Key Properties for Positioning:**
- **`position`**: Defines the positioning method.
- **`top`, `right`, `bottom`, `left`**: Define the offset of an element.
- **`z-index`**: Controls the stacking order of elements.

---

## **9. Background Image in CSS**

A **background image** is used to set an image as the background of an HTML element.

### **CSS Background Properties:**
- **`background-image`**: Specifies the image to be used as the background.
- **`background-size`**: Controls the size of the background image (e.g., `cover`, `contain`).
- **`background-position`**: Defines the starting position of the background image (e.g., `center`, `top left`).
- **`background-repeat`**: Controls whether the background image repeats (e.g., `no-repeat`, `repeat`).

---

## **10. Display and Alignment in CSS**

### **Display Property:**
The `display` property in CSS defines the layout behavior of an element.

- **`block`**: The element takes up the full width available, and the next element is displayed on a new line.
- **`inline`**: The element only takes up as much width as necessary and does not start on a new line.
- **`inline-block`**: Similar to `inline`, but allows setting width and height.
- **`none`**: The element is removed from the document flow (it will not be displayed).

### **Alignment in CSS:**
Alignment helps position elements relative to each other.

- **`text-align`**: Aligns inline content (like text or inline-block elements) horizontally within a block container. Values include `left`, `center`, `right`, and `justify`.
- **`vertical-align`**: Aligns inline or inline-block elements vertically within a line (e.g., `top`, `middle`, `bottom`).
- **`justify-content`**: Aligns items in a flex container along the main axis (horizontal for `row`, vertical for `column`).
- **`align-items`**: Aligns items in a flex container along the cross axis (perpendicular to the main axis).

---

## **Conclusion**

Understanding HTML and CSS fundamentals is essential for web development. HTML provides the structure, while CSS enhances the presentation and layout. By mastering both, you can create well-structured and visually appealing websites.

---
