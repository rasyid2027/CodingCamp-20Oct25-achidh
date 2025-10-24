# NexaTech - Modern Futuristic Company Profile Website

A stunning, modern company profile website with a futuristic design featuring glassmorphism effects, animated gradients, comprehensive JavaScript form validation, and a complete profile page.

## 📋 Project Requirements Completed

✅ **1. Profile Page with Complete Information**
- Photo banner with company stats
- About the company section with highlights
- Vision and Mission section with detailed points
- Core values section (6 values)
- Leadership team section

✅ **2. Navigation to Profile Page**
- "Our Profile" link in navbar
- Smooth navigation between pages

✅ **3. Welcome Message with JavaScript**
- "Hi [Name]" greeting on home page
- Name input with localStorage persistence
- Dynamic name display

✅ **4. Form Validation & Value Display**
- Complete JavaScript validation for all fields
- Display submitted values in HTML after form submission
- Real-time validation feedback

✅ **5. Responsive Design**
- Fully responsive on Desktop (1200px+)
- Tablet optimized (768px - 1199px)
- Mobile optimized (below 768px)

✅ **6. Organized File Structure**
- CSS in `css/style.css` (single file)
- JavaScript in `js/script.js` (single file)
- Clean, maintainable code structure

## 🚀 Features

### Design & UI/UX
- **Modern Futuristic Design**: Cutting-edge visual design with cyberpunk-inspired elements
- **Glassmorphism Effects**: Beautiful frosted glass effects on cards and components
- **Animated Background**: Dynamic gradient orbs and grid overlay animations
- **Smooth Animations**: Fade-in, slide-in, and floating animations throughout
- **Responsive Design**: Fully responsive across all devices (desktop, tablet, mobile)
- **Interactive Elements**: Hover effects, transitions, and micro-interactions

### Pages & Sections

#### Home Page (index.html)
1. **Welcome Section**: Personalized greeting with name input (JavaScript powered)
2. **Hero Section**: Eye-catching introduction with animated floating cards
3. **About Section**: Company overview with animated statistics counter
4. **Services Section**: Showcase of 6 core services with feature tags
5. **Contact Section**: Contact information and validated inquiry form with value display
6. **Footer**: Company links and social media

#### Profile Page (profile.html)
1. **Photo Banner**: Hero banner with company founding stats
2. **About the Company**: Detailed company information with highlights
3. **Vision & Mission**: Comprehensive vision and mission statements with bullet points
4. **Core Values**: 6 core company values with descriptions
5. **Leadership Team**: Team member profiles with roles
6. **Call to Action**: Engagement section with links

### Form Validation
Comprehensive JavaScript validation for the contact form:

#### Name Field
- ✅ Required field
- ✅ Minimum 2 characters
- ✅ Maximum 50 characters
- ✅ Only letters and spaces allowed
- ✅ Real-time validation

#### Email Field
- ✅ Required field
- ✅ Valid email format (user@domain.com)
- ✅ Pattern matching with regex
- ✅ Real-time validation

#### Phone Number Field
- ✅ Required field
- ✅ Minimum 10 digits
- ✅ Maximum 20 characters
- ✅ Accepts numbers, spaces, dashes, plus signs, and parentheses
- ✅ Auto-formatting (US format)
- ✅ Real-time validation

#### Message Field
- ✅ Required field
- ✅ Minimum 10 characters
- ✅ Maximum 500 characters
- ✅ Real-time validation

### Validation Features
- **Real-time Feedback**: Validates on blur, focus, and input events
- **Error Messages**: Clear, specific error messages for each validation rule
- **Visual Indicators**: Red border and shake animation for errors
- **Success Message**: Animated success confirmation after submission
- **Display Submitted Values**: Shows all submitted form data in HTML
- **Accessibility**: ARIA labels and screen reader announcements
- **Form Reset**: Automatic form reset after successful submission

### Welcome Message Features
- **Name Input**: Collects user name on first visit
- **LocalStorage**: Persists name across page refreshes
- **Dynamic Greeting**: "Hi [Name]!" displayed with animation
- **Enter Key Support**: Submit name with Enter key

## 🛠️ Technologies Used

- **HTML5**: Semantic markup with two pages
- **CSS3**: Modern styling with custom properties, flexbox, and grid
- **JavaScript (Vanilla)**: No frameworks, pure JavaScript for maximum performance
- **LocalStorage API**: For name persistence
- **Google Fonts**: Orbitron and Rajdhani fonts for futuristic typography

## 📁 File Structure

```
revou/
│
├── index.html          # Home page with welcome message and contact form
├── profile.html        # Company profile page
├── css/
│   └── style.css       # Single CSS file for all styling
├── js/
│   └── script.js       # Single JavaScript file for all functionality
└── README.md           # Project documentation
```

## 🚀 Getting Started

### Installation

1. Clone or download the project files
2. No build process required - it's pure HTML, CSS, and JavaScript!

### Running the Website

Simply open `index.html` in your web browser:

```bash
# Option 1: Double-click index.html

# Option 2: Use a local server (recommended)
# Python 3
python -m http.server 8000

# Node.js (with http-server)
npx http-server

# VS Code Live Server extension
# Right-click index.html > Open with Live Server
```

Then navigate to `http://localhost:8000` in your browser.

## 🎨 Color Scheme

The website uses a modern, futuristic color palette:

- **Primary**: Cyan (#00f0ff) - Main accent color
- **Secondary**: Purple (#7b2ff7) - Secondary accent
- **Accent**: Pink (#ff006e) - Call-to-action elements
- **Success**: Green (#00ff88) - Success states
- **Background**: Dark blue (#0a0e27, #050814) - Main backgrounds
- **Text**: White (#ffffff) and Gray (#94a3b8)

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

## ✨ Key Features Explained

### 1. Animated Background
Three gradient orbs float and move in the background with a grid overlay, creating a dynamic, futuristic atmosphere.

### 2. Statistics Counter
Numbers animate from 0 to their target value when the stats section comes into view using Intersection Observer API.

### 3. Smooth Scrolling
Navigation links smoothly scroll to their respective sections with active state highlighting.

### 4. Form Validation System
A robust validation system that:
- Validates each field individually
- Shows errors immediately on blur
- Clears errors on focus
- Provides real-time feedback during typing
- Prevents submission if validation fails
- Displays success message on successful submission

### 5. Mobile Navigation
Hamburger menu for mobile devices with smooth slide-in animation.

## 🔧 Customization

### Changing Colors
Edit the CSS custom properties in `styles.css`:

```css
:root {
    --primary-color: #00f0ff;
    --secondary-color: #7b2ff7;
    /* ... other colors */
}
```

### Modifying Content
Edit the HTML content in `index.html` to match your company information.

### Adjusting Validation Rules
Modify the `validationRules` object in `script.js`:

```javascript
const validationRules = {
    name: {
        required: true,
        minLength: 2,
        // ... other rules
    }
};
```

## 🌟 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## 📝 Form Submission

Currently, the form logs data to the console. To connect to a backend:

1. Uncomment the `submitFormData()` function in `script.js`
2. Update the API endpoint
3. Handle the response accordingly

Example:
```javascript
fetch('/api/contact', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(formData),
})
```

## 🎯 Performance Optimizations

- Debounced scroll events
- Intersection Observer for animations
- CSS transforms for smooth animations
- Minimal JavaScript dependencies
- Optimized CSS with custom properties

## 📄 License

This project is open source and available for educational purposes.

## 👨‍💻 Author

Created as a mini project for RevoU Software Engineering course.

## 🤝 Contributing

Feel free to fork this project and customize it for your needs!

---

**Built with ❤️ using modern web technologies**
