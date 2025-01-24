# About Us Section

This project is a responsive "About Us" section for a website, featuring a Bootstrap-based carousel. The carousel displays multiple items dynamically depending on the screen size, ensuring an optimized user experience on desktop, tablet, and mobile devices.

## Features

1. **Responsive Design**:
   - Desktop: Displays 3 services/images at a time.
   - Tablet: Displays 2 services/images at a time.
   - Mobile: Displays 1 service/image at a time.

2. **Carousel Functionality**:
   - Automatically slides every 2 seconds.
   - Allows manual navigation via previous/next buttons.

3. **Customizable Content**:
   - Each carousel item includes an image and an overlay caption with a title and description.

## Technologies Used

- **HTML**: Structure of the About Us section.
- **CSS**: Custom styling for the carousel and responsiveness.
- **Bootstrap**: Carousel component and grid system.
- **JavaScript**: Bootstrap's built-in carousel functionality.

## File Structure

```plaintext
project-folder/
|-- index.html         # Contains the About Us section code.
|-- images/about/      # Folder containing carousel images.
|-- README.md          # Documentation for the project.
```

## How to Use

1. **Setup Bootstrap**:
   - Ensure Bootstrap CSS and JS files are included in your project. Use the following CDN links in the `<head>` and before the closing `<body>` tag:
     ```html
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
     ```

2. **Replace Images**:
   - Add your images to the `images/about/` folder and update the `src` attributes in the `<img>` tags.

3. **Customize Text**:
   - Modify the titles (`<h5>`) and descriptions (`<p>`) within the `carousel-caption` divs to match your content.

4. **Test Responsiveness**:
   - Open the project in a browser and resize the window to test how the carousel adapts to different screen sizes.

## Customization

- **Carousel Timing**: Adjust the sliding interval (currently 2 seconds) by adding the `data-bs-interval` attribute to the carousel element:
  ```html
  <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel" data-bs-interval="2000">
  ```

- **Number of Items**: Add or remove `<div class="carousel-item">` blocks as needed.

## Example Code Snippet

```html
<div class="carousel-item col-12 col-sm-6 col-md-4 col-lg-2 active">
    <img src="./images/about/about-img.jpg" class="img-fluid d-block w-100" alt="...">
    <div class="carousel-caption d-none d-md-block">
        <h5>Our Mission</h5>
        <p>Delivering excellence and innovation in every aspect of our business.</p>
    </div>
</div>
```

## Credits

- **Bootstrap**: [https://getbootstrap.com/](https://getbootstrap.com/)
- Placeholder images sourced from project assets.

## License

This project is open-source and available under the [MIT License](LICENSE).
