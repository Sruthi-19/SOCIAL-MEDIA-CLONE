Initially home page will be rendered
Add button will be present in home page
On click of add button a drop down will be displayed
Drop down will contain options like story post etc
Here we will be doing only post
On click of the post option from dropdown, File explorer will be opened
As of now functionality will be developed to add only image as post.
On selecting the image, from home page it will be redirected to post preview page.
In post preview page the selected image will be displayed
A text box with add caption placeholder will be there.
Finally a post button is present.
On clicking the post button the user will be redirected to the home page
Now the home page will be re rendered with the image and the caption.
This time the caption will not be editable. It will be like a text
Along with image and caption edit button will be present for every post.
On clicking the edit button same preview page with image and caption text box will be displayed.
The existing caption will be displayed in the box (it will not be empty like first when we post).
Instead of post button, update post button will be present.
Onclick of update, the home page will be re rendered with updated caption.

REACT FUNCTIONALITIES:

1. App Component will be rendered in Main jsx file.
2. It will contain all routes -> Home and Preview page
3. The states will also be present in App component
4. Context is used and the provider will wrap the routes so that the states can be passed
5. Home Component:
   5.1 Button on click -> display dropdown
   5.2 The value of drop down will be like buttons(something like input tag type file - need to search other alternatives).
   5.3 Onclick of post (input accept image) file explorer will pop up
   5.4 And the post button will redirect to preview page.
   5.5 Inside the input tag on change function will be written.
   5.6 State for current image URL, overall images array(more than one post)
   5.7 The state for current image will be updated and the image in preview page with caption will be rendered.

   STATES:

   1. Current Image url -> For preview page -> on change in image upload
   2. Ovarll images and caption JSON array -> Map and render in home page
   3. Current caption -> on change in caption input box
   4. Edit Icon click -> Conditional rendering for preview page

   ROUTES:
   1. Home page
   2. Post button (inside dropdown) -> Preview page
   3. In preview page (Post button) -> Home page
   4. Edit icon -> Preview page
