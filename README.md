# Bean-Voyage

Welcome to Bean Voyage, a modern and interactive coffee shop website that offers a seamless user experience for coffee enthusiasts. This project showcases the best coffee options from around the world, complete with a stylish design and intuitive functionality.

Table of Contents :-

Features
Technologies Used
Installation
Usage
JavaScript Functionality
Contributing
Author

Features:-

Responsive Navigation Bar: The navigation bar toggles on smaller screens and closes automatically when interacting with other elements or scrolling.
Interactive Search Form: The search form is easily accessible and can be toggled with a click.
Dynamic Shopping Cart: A user-friendly shopping cart that can be opened or closed with a single click.
Smooth Animations: Interactive UI elements with smooth transitions and animations for a polished look.
Product Sections: Display various coffee products with images, descriptions, and prices.
Social Media Links: Connect with us via social media integrated into the website footer.
Mobile-Friendly Design: Optimized for all devices including desktops, tablets, and mobile phones.

Technologies Used :-

HTML5: Markup language for creating the structure of the website.
CSS3: Styling for the layout, responsiveness, and interactive features:
Flexbox & Grid: For arranging elements in a responsive and adaptable manner.
Media Queries: Ensures that the design adapts to various screen sizes.
Custom CSS Variables: For consistent and maintainable styling.
JavaScript: Adds dynamic behavior and interactivity:
DOM Manipulation: Toggle functionality for the navigation bar, search form, and shopping cart.
Event Listeners: For handling clicks and scroll events to manage UI state.

Installation :-

To run this project locally, follow these steps:

Clone the Repository

bash
Copy code
git clone https://github.com/yourusername/bean-voyage.git
Navigate to the Project Directory

bash
Copy code
cd bean-voyage
Open the Project in Your Browser

Open the index.html file in your browser by double-clicking or using a live server extension in your code editor.

Usage :-

Once you have the project set up, you can explore these functionalities:

Navigate through the Menu: Explore different sections of the website using the responsive navigation bar.
Search for Products: Use the search form to filter and find specific products.
View the Cart: Click on the shopping cart icon to view selected items, and close it when done.
Explore Products: Browse through our delicious coffee offerings, complete with descriptions and prices.
Responsive Design: Enjoy a seamless experience on all devices, from desktops to mobile phones.

JavaScript Functionality :-

The website features JavaScript that powers the interactive UI elements:

Navbar Toggle: Clicking the menu button (#menu-btn) toggles the navigation bar on mobile devices. The navbar closes when another interactive element (like the search form or cart) is opened.

javascript
Copy code
document.querySelector('#menu-btn').onclick = () => {
    navbar.classList.toggle('active');
    searchForm.classList.remove('active');
    cartItem.classList.remove('active');
};
Search Form Toggle: Clicking the search button (#search-btn) toggles the visibility of the search form. It automatically closes the navbar and cart if they are open.

javascript
Copy code
document.querySelector('#search-btn').onclick = () => {
    searchForm.classList.toggle('active');
    navbar.classList.remove('active');
    cartItem.classList.remove('active');
};
Cart Toggle: Clicking the cart button (#cart_btn) opens or closes the shopping cart. Like the search form, it ensures that the other elements (navbar and search form) close when the cart is open.

javascript
Copy code
document.querySelector('#cart_btn').onclick = () => {
    cartItem.classList.toggle('active');
    navbar.classList.remove('active');
    searchForm.classList.remove('active');
};
Close on Scroll: As soon as the user scrolls the page, the navbar, search form, and cart automatically close to maintain a clean and clutter-free view.

javascript
Copy code
window.onscroll = () => {
    navbar.classList.remove('active');
    searchForm.classList.remove('active');
    cartItem.classList.remove('active');
};

Contributing :-

If you would like to contribute to this project, follow these steps:

Fork the Repository

Create a New Branch

bash
Copy code
git checkout -b feature/your-feature-name
Commit Your Changes

bash
Copy code
git commit -m "Add your changes"
Push to the Branch

bash
Copy code
git push origin feature/your-feature-name
Open a Pull Request


Author
Akshat Dubey

Thank you for checking out Bean Voyage. We hope you enjoy exploring the website as much as we enjoyed creating it!

