# Frontend Mentor | QR Code Component Solution

This is a solution to the **QR code component** challenge on [Frontend Mentor](https://www.frontendmentor.io). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

![Preview](./preview.jpg)

### The Challenge

Your users should be able to:

- View the optimal layout depending on their device's screen size.
- See a QR code image and related text in a responsive layout that adjusts to both mobile and desktop devices.

### Screenshot

![Design Preview](./design/desktop-design.jpg)

## My Process
 I begun buidling the HTML first and follwed with the CSS structuring
### Built With

- Semantic HTML5 markup
- CSS Flexbox
- Mobile-first workflow

### What I Learned

In this project, I practiced working with **CSS Flexbox** to make the layout responsive. I also explored using the **Google Fonts** API to import custom fonts (Outfit) and optimized image scaling with CSS properties such as `max-width`, `flex-grow`, and `flex-shrink`.

Here's a sample of the CSS code that helped me handle the image responsiveness:

```css
#qr-code img {
    border-radius: 10px;
    height: auto;
    max-width: 100%; /* Image will not exceed the width of its container */
    flex-grow: 1; /* Allows the image to grow if space allows */
    flex-shrink: 1; /* Allows image to shrink if the container is small */
} 
@media(max-width: 375px){
    #container{
        max-width: 200px;
    }
}
/* Desktop view - 1440px*/
@media(max-width: 1440px){
    #container{
        max-width: 250px;
    }
}
