# READ12


- EJS Partials help us avoid repetition of the same code on several web pages.

- EJS partials work like EJS layouts too in creating a single fix content on a web page.

- Unlike EJS Layouts, EJS partials can work without the express-ejs-layouts module. EJS partials apply in cases like creating objects like header, footer, div.

- Linking Partials in Templates
   <% include templateName %>


This new command **includ** is telling Express to pull the contents of the named template and place it in place of this command.

We know that Express is already looking in the views directory for our templates, so when we give the name of the template to be included we consider that to be the root directory, but we still have to tell it to look in the partials folder that we made. so our template name would look like this.

<% include partials/header.ejs %>