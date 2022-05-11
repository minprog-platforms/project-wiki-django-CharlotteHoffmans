# Application Name

Shows encyclopedia entries. 


## Getting Started
-> make entry page:
![Entry page](/image/entry.jpeg)
    The entry page shows the topic and the information about it. 
    
    In url patterns add the path("<str:title>", views.entry, title="title")
    in views add a def to get the html page for that title, in view use the appropriate util funcstion.

-> Index Page:
    Shows the titles available, the option to search, choose a random title and to add a new page. When the user clicks on any entry name it will go to that entry page. 
    
    Make from all the options links, that can go to the right pages. 

-> Search: 
    The search box allow the user to type a query into the search box in the sidebar to search for an encyclopedia entry. If the query matches the name of an encyclopedia entry, the user should be redirected to that entry’s page. If the query does not match the name of an encyclopedia entry, the user should instead be taken to a search results page that displays a list of all encyclopedia entries that have the query as a substring. Clicking on any of the entry names on the search results page should take the user to that entry’s page. 
    
    Add all the options in the search box in layout.html

-> New Page:
![New page page](/image/new_page.jpeg)
    Clicking “Create New Page” in the sidebar takes the user to a page where they can create a new encyclopedia entry.
    When the page is saved, if an encyclopedia entry already exists with the provided title, the user is  presented with an error message.
    Otherwise, the encyclopedia entry should be saved to disk, and the user should be taken to the new entry’s page.

    Add a new path new_page, in view add a def that shows a new html file. Add a new path, change_title, add in view a def that post the content that was made in change_title. 

-> Edit Page (extra): 
![Edit page](/image/edit.jpeg)
    On each entry page, the user should be able to click a link to be taken to a page where the user can edit that entry’s Markdown content in a textarea.

    add a new path change_content and in view a def that post the new content on the allready existing page.

-> Random Page (extra): 
    Clicking “Random Page” in the sidebar should take user to a random encyclopedia entry.

    Make from random Page a link that goes to a random page. 

-> Markdown to HTML Conversion: 
    On each entry’s page, any Markdown content in the entry file should be converted to HTML before being displayed to the user. Download the python-markdown2 package to perform this conversion, installable via pip3 install markdown2.


