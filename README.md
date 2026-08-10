# 🌍 Tourvia – Travel Website

Tourvia is a modern and responsive travel website designed for travelers who want to explore destinations, discover curated tour packages, and experience seamless travel planning.

The website is built using **HTML, CSS, Bootstrap, and JavaScript**, with a visually rich travel-focused design featuring destination cards, tour packages, testimonials, videos, blogs, and interactive hover effects.

## ✨ Features

* 🏠 Modern Hero Section
* 🧭 Responsive Navigation Bar
* 🌄 Travel Destination Showcase
* ✈️ Popular Destinations
* 🎒 Exclusive Tour Packages
* ⭐ Customer Testimonials
* 🏨 Tour Activities & Experiences
* 🎥 Full-Screen Travel Video Section
* 📝 Travel Blog Section
* 📱 Responsive Design
* 🎨 Modern Hover Animations
* 🦶 Responsive Footer Section

## 🛠️ Technologies Used

* **HTML5** – Website structure
* **CSS3** – Styling, animations, layouts, and responsive design
* **Bootstrap 5.3.8** – Responsive grid and UI components
* **JavaScript** – Scroll-based tour card animation
* **SVG** – Icons and logos
* **WebP / MP4** – Images and travel videos

Bootstrap 5.3.8 is included through the Bootstrap CDN in the project.

## 📂 Project Structure

```text
Tourvia/
│
├── index.html
├── style.css
│
├── assest/
│   ├── tourvia-logo.svg
│   ├── favicon.svg
│   ├── arrow.svg
│   ├── arrow-white.svg
│   ├── mountain-img.webp
│   ├── hero-bg-image.webp
│   ├── vedio.mp4
│   ├── explore.mp4
│   ├── destination-img.webp
│   ├── canada.webp
│   ├── dubai.webp
│   ├── rating.webp
│   ├── merlion-park.webp
│   ├── grand canal.webp
│   ├── testimonials-img.webp
│   ├── tour-img.webp
│   ├── blog images
│   └── other icons and assets
│
└── README.md
```

> Make sure the `assest` folder is present in the same project directory because the HTML and CSS files reference images, icons, and videos from this folder.

## 🏠 Website Sections

### 1. Hero Section

The hero section introduces Tourvia with:

* Tourvia branding
* Navigation menu
* Welcome message
* Main heading
* Explore Destination button
* Travel video card
* Mountain visual

The hero uses a full-screen background image with a dark overlay for better text visibility.

### 2. About Us

The About section introduces Tourvia and displays travel statistics such as:

* Happy Travelers
* Customer Satisfaction
* Supporting travel images

The HTML includes statistics of **5707+ happy travelers** and **170% customer satisfaction**.

### 3. Popular Destinations

The destination section showcases popular travel destinations:

* 🇯🇵 Japan – Imperial Tokyo
* 🇨🇦 Canada – Kananaskis Country
* 🇦🇪 Dubai – Burj Khalifa

Destination cards include images, location names, visited-place counts, and hover effects.

### 4. Why Choose Us

This section explains why travelers should choose Tourvia and highlights:

* Curated travel experiences
* Seamless booking
* Secure reservation process
* Customer review

### 5. Tour Packages

The Tour Package section displays exclusive packages including:

* **Merlion Park**
* **Grand Canal**
* Package location
* Starting price
* Number of days
* Package details button

### 6. Testimonials

A testimonial section allows customers to share their travel experiences with Tourvia.

It includes:

* Five-star rating
* Customer review
* Customer name
* Traveler image

### 7. Tour Activities

The Tour Activities section presents curated experiences such as:

* Exclusive Residences
* Exceptional Packages
* Seamless Booking

The information cards are positioned dynamically using JavaScript based on page scrolling.

### 8. Explore Video Section

A full-screen video section provides an immersive travel experience with:

* Background travel video
* Play button
* Animated **EXPLORE NOW** marquee text

The CSS creates a continuous marquee animation using `@keyframes`.

### 9. Travel Blog

The blog section contains travel-related articles and image cards, including:

* Travel category
* Blog images
* Article titles

### 10. Footer

The footer contains:

* Quick Links
* Social Media links
* Explore Destination button
* Copyright information
* Style Guide
* Licenses
* Changelog
* Tourvia branding

## 📱 Responsive Design

The website uses Bootstrap's responsive grid system along with CSS media-query-based styling to adapt the layout for different screen sizes.

The project also uses responsive CSS functions such as `clamp()` for scalable typography.

## 🎨 UI & Animation

The website includes several visual effects:

* Button hover animations
* Destination image zoom
* Card hover effects
* Video-card hover animation
* Blog image zoom
* Tour information card animation
* Continuous Explore Now marquee
* Scroll-based positioning of tour cards

For example, destination images scale when the user hovers over a destination card.

## ⚙️ JavaScript Functionality

JavaScript is used to dynamically change the position of the tour information cards while scrolling.

```javascript
window.addEventListener('scroll', () => {
    const rect = tourSection.getBoundingClientRect();
    const windowHeight = window.innerHeight;

    const progress =
        (windowHeight - rect.top) /
        (windowHeight + rect.height);

    const clamped = Math.min(Math.max(progress, 0), 1);

    cards.forEach(card => {
        if (!card.el) return;

        const topPercent =
            card.start -
            (clamped * (card.start - card.end));

        card.el.style.top = topPercent + '%';
    });
});
```

This functionality is implemented directly in the HTML file.

## 🚀 How to Run

1. Download or clone the project.
2. Open the project folder in VS Code.
3. Make sure the `assest` folder is present.
4. Open `index.html` in your browser.

For the best development experience, you can use the **Live Server** extension in VS Code.

## 📸 Project Preview

Add your project screenshot here:

```markdown
![Tourvia Website Preview](./screenshot.png)
```

## 🔮 Future Improvements

Possible future improvements include:

* Add real destination search
* Add working booking functionality
* Add destination detail pages
* Add package filtering
* Add contact form functionality
* Add user authentication
* Connect the website to a backend
* Add a database for tour packages
* Add online payment functionality
* Make navigation links fully functional

## 👩‍💻 Author

**Muskan Kishnani**

BCA Student | Full Stack Web Development Learner

### Skills Used

`HTML` `CSS` `Bootstrap` `JavaScript` `Git` `GitHub`

---

⭐ If you like this project, consider giving it a star on GitHub!
