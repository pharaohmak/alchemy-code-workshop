# HTML

## Elements and Structure

### intro to html

REVIEW
- HTML = HyperTextMarkupLanguage
- used to create the structure and content of a webpage
- most html elements contain opening and closing tags with raw text or other html tags between them 
- html elements can be nested inside other elements. the enclosed element is the child of the enclosing parent element
- any visable content should be placed within the opening and closing <body> tags
- headings and sub-headings, <h1> to <h6>, are used to provide titles for sections of content
- <p>, <span>, and <div> tags specify text or blocks
- the <em> and <strong> tags are used to emphasize text
- line breaks are created using the <br> tag
- ordered lists (<ol>) are numbered and unordered lists (<ul>) are bulleted
- images (<img>) and videos (<video>) can be added by linking to an existing source
    

### HTML Document Standards
    
- the <!DOCTYPE html> declaration should always be the first line of code in your html files. This lets the browser know what version of html to expect
- the <html> element will contain all of your html code
- information about the web page, like the title, belongs within the <head> of the page
- you can add a title to your web page by using the <title> element, inside of the head
- a webpage's title appears in a browser's tab
- anchor tags (<a>) are used to link to internal pages, external pages or content on the same page
- you can create sections on a webpage and jump to them using <a> tags and adding id's to the elements you wish to jump to
- whitespace between html elements helps make code easier to read while not changing how elements appear in the browser
- indentation also helps make code easier to read. it makes parent-child relationships visible


## Tables

### HTML tables
    - the <table> element creates a table 
    - the <tr> element adds rows to a table
    - to add data to a row, you can use the <td> element
    - table headings clarify the meaning of data. headings are added with the <th> element
    - table data can span columns using the colspan arrtibute
    - table data can span rows using the rowspan attribute
    - tables can be split into three sections: a head, a body, and a footer
    - a tables head is created with the <thead> element 
    - the body is created with the <tbody> element
    - the tables footer is created with the <tfoot> element


## Forms

### HTML forms
    - the purpose of a <form> is to allow users to input information and send it
    - the <form> action attribute determines where the forms information goes
    - the <form> method attribute determines how the information is sent and processed
    - to add fields for users to input information we use the <input> element and set the type attribute to a field;
        - "text" : creates a single row field for text input
        - "password" : creates a single row field that censors text input
        - "number" : creates a single row field for number input
        - "range" : creates a slider to select from a range of numbers
        - "checkbox" : creats a single checkbox which can be paired wih other cheboxes
        - "radio" : creates a radio button that can be paired with other radio buttons
        - "list" : will pair the <input> with a <datalist> element if the id of both are the same
        - "submit" : creates a submit button
    - a <select> element is populated with <option> elements and renders a dropdown list selection
    - a <datalist> element is populated with <option> elements and works with an <input> to search through choices
    - a <textarea> element is a text input field that has a customizable area
    - when a <form> is bubmitted, the name of the fields that accept input and the calue of those fields are sent as name=value pairs

    
### HTML validation
    - client-side calidations happen in the browser before the information is sent to the server
    - adding the required attribute to an input related element will validate that the input field has information in it
    - assigning a value to the min attribute of a number input element will validate an acceptable minimum number 
    - assigning a value max attribute of a number input element will validate an acceptable maximum value
    - assigning a value to the minlength attribute of a text input element will validate an acceptable minimum number of characters
    - assigning a maxlength attribute of a text input element will validate an acceptable maximum number of characters
    - assigning a regex to pattern matches the input to the provided regex
    - if validations on a <form> do not pass, the user gets a message explaining why and the <form> cannot be submitted
    


## Semantic HTML

### semantic HTML
    - introduces meaning to a page through specific elements that provide context as to what is in between the tags
    - semantic html is a modern standard and makes a website accessible for people who use screen readers to translate the webpage and improves your website's SEO
    - <header>, <nav>, <main>, and <footer> create the basic structure of the webpage
    - <section> defines elements in a document, such a chapters, headings, or any other area of the document with the same theme
    - <article> holds content that makes sense on its own such as articles, blogs, comments, etc. 
    - <aside> contains information that is related to the main content, but not required in order to understant the dominant information
    - <figure> encapulates all types of media
    - <figcaption> is used to describe the media in <figure>
    - <video>, <embed>, and <audio> are used for media files