# SnapSyntax

# Modern Shopping Experience

A responsive, interactive shopping website showcasing various product categories with dynamic color themes and hover effects.

## Overview

This project is a front-end implementation of a modern e-commerce website that features a clean and elegant design with interactive elements. The website changes theme colors based on the category being viewed and includes smooth transitions and hover effects to enhance user experience.

## Features

- **Dynamic Color Themes**: Background colors change based on the selected product category
- **Interactive Product Cards**: Product cards feature hover animations with image blur effects and information displays
- **Responsive Design**: Fully responsive layout that works well on both desktop and mobile devices
- **Category Navigation**: Fixed side navigation dots for quick access to different product sections
- **Video Integration**: Supports video previews for each product that appear on hover
- **Smooth Scrolling**: Implemented smooth scrolling for better navigation experience

## Technologies Used

- HTML5
- CSS3 (with CSS Variables, Flexbox, and CSS Grid)
- Vanilla JavaScript (minimal)

## Project Structure

```
modern-shopping-website/
├── index.html
├── styles.css
├── README.md
└── images/
    ├── image1.avif
    ├── image2.avif
    ├── image3.avif
    ├── image4.avif
    ├── image5.avif
    ├── image6.avif
    └── image7.avif
```

## Setup and Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/modern-shopping-website.git
   ```

2. Navigate to the project directory:
   ```
   cd modern-shopping-website
   ```

3. Open `index.html` in your browser to view the website.

## Customization

### Adding New Categories

To add a new product category:

1. Add a new section in the HTML with appropriate ID and class
2. Create a new color variable in the CSS `:root` selector
3. Add the corresponding CSS for target-based color changes
4. Update the category navigation with a new link

Example:

```html
<section id="new-category" class="category-section">
    <div class="product-box" data-category="new-category">
        <!-- Content here -->
    </div>
</section>
```

```css
:root {
    /* Add new color variable */
    --color-new: #yourhexcode;
}

/* Add target-based color change */
#new-category:target ~ #page-container,
#new-category:target {
    background-color: var(--color-new);
}
```

## Browser Compatibility

The website is compatible with:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Future Enhancements

- Add shopping cart functionality
- Implement product filtering and search
- Add product detail pages
- Integrate backend functionality for actual e-commerce capabilities
- Add user account management

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Design inspiration from modern luxury brand websites
- Images used are placeholder avif files and should be replaced with your own content