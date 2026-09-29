<div align="center">

# ✨ Vihaan Khanna | Portfolio

**A dynamic, multi-page personal portfolio built with pure HTML, CSS and JavaScript.**
No frameworks. No build step. Just one file that runs anywhere.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Dependencies](https://img.shields.io/badge/dependencies-0-20c997?style=for-the-badge)

[**Live Demo**](#-live-demo) · [**Features**](#-features) · [**Getting Started**](#-getting-started) · [**Customize**](#-customization-guide) · [**Deploy**](#-deployment)

</div>

---

## 📸 Preview

> Add a screenshot or GIF of your site here.
> Save it as `preview.png` in the project folder, then uncomment the line below.

<!-- ![Portfolio preview](preview.png) -->

## 🌐 Live Demo

🔗 **[your-username.github.io/portfolio](https://your-username.github.io/portfolio)**
*(Replace this link once you have deployed the site.)*

---

## 🚀 Features

### 🎨 Design
- **Glassmorphism UI** with frosted cards and a floating navigation bar
- **Animated particle network** in the background that reacts to your mouse
- **Floating colour blobs** and a **cursor glow** for depth
- **Gradient animated name** on the hero section
- **Fully responsive** layout for phones, tablets and desktops

### ⚡ Interactivity
| Feature | Where | What it does |
|---|---|---|
| Typing effect | Home | Cycles through roles like "IoT Tinkerer" |
| Animated counters | Home | Stats count up when the page loads |
| Magnetic buttons | Home / Contact | Buttons drift toward your cursor |
| Tabbed sections | About | Switch between Skills, Journey and Interests |
| Animated skill bars | About | Bars fill smoothly when shown |
| Live project search | Projects | Filters cards as you type |
| Category filters | Projects | All / IoT / Web / AI |
| 3D tilt cards | Projects | Cards tilt following your cursor |
| Project modals | Projects | Popup with details and what you learned |
| Form validation | Contact | Checks name, email and message length |
| Copy email button | Contact | Copies your email to the clipboard |
| Toast notifications | Everywhere | Small feedback popups |

### 🎛️ Personalisation for visitors
- **Dark / Light mode** toggle (also follows the system setting)
- **4 accent colours** to choose from
- **Remembers preferences** using `localStorage`
- **Scroll progress bar** at the top of the page

### ⌨️ Keyboard shortcuts
| Key | Action |
|---|---|
| `1` | Go to Home |
| `2` | Go to About |
| `3` | Go to Projects |
| `4` | Go to Contact |
| `Esc` | Close the project popup |

---

## 🛠️ Tech Stack

| Technology | Used for |
|---|---|
| **HTML5** | Structure and semantic markup |
| **CSS3** | Layout (Grid and Flexbox), animations, glass effects, theming with CSS variables |
| **JavaScript (ES6+)** | Routing, rendering, animations, canvas particles, form logic |
| **Canvas API** | The particle network background |
| **localStorage** | Saving theme and accent colour |
| **Google Fonts** | *Space Grotesk* (falls back to system fonts if offline) |

---

## 📁 Project Structure

The whole site lives in a single file:

```
portfolio/
├── index.html     # HTML + CSS + JS, everything in one file
└── README.md      # You are here
```

> The file was generated as `portfolio-website.html`. **Rename it to `index.html`** before deploying so hosts open it automatically.

---

## ⚙️ Getting Started

### Run locally

1. **Download** the project (or clone the repository):
```bash
   git clone https://github.com/your-username/portfolio.git
   cd portfolio
```
2. **Open `index.html`** in any modern browser (double-click it).

That's it. There is nothing to install.

### Optional: use a local server

For a more realistic test, run a tiny server:

```bash
# Python 3
python -m http.server 8000
```

Then visit `http://localhost:8000`.

---

## 🧩 Customization Guide

Everything you would want to edit is inside the `<script>` section at the bottom of `index.html`.

### 1. Change your contact email

```js
const EMAIL = 'you@example.com';   // ← put your real email here
```

### 2. Edit your skills

```js
const SK = [['HTML', 80], ['CSS', 75], ['Java', 35], ['C++', 35], ['Arduino', 55]];
//           name   percent
```

### 3. Add or edit projects

Each project is one object in the `PJ` array:

```js
{
  id: 5,                      // unique number
  c: 'web',                   // category: 'iot', 'web' or 'ai'
  i: '🚀',                    // emoji icon
  t: 'My New Project',        // title
  d: 'One-line description.', // shows on the card
  tech: ['HTML', 'CSS'],      // tags
  more: 'Longer description shown in the popup.',
  learn: 'What you learned from building it.'
}
```

### 4. Change the typing roles

```js
const roles = ['CSE (AI/ML) Student', 'Web Developer in the making', 'IoT Tinkerer', 'Hackathon Enthusiast'];
```

### 5. Edit your interests

```js
const IN = [['🤖', 'AI & ML', 'Short note shown when tapped.'], /* ... */];
```

### 6. Change accent colours

```js
const AC = ['#6c5ce7', '#00b8d9', '#f76707', '#12b886'];
```

### 7. Update text, stats and social links

- **Home stats:** edit the `data-to="..."` numbers in the `.stats` block.
- **Timeline:** edit the entries inside `<div id="jo">` in the About section.
- **GitHub / LinkedIn:** replace the placeholder text in the Contact section.
- **Page title and footer name:** search for `Vihaan Khanna` and update as needed.

---

## 🌍 Deployment

### Option A: GitHub Pages (free)

1. Create a new repository on GitHub.
2. Upload `index.html` and `README.md`.
3. Go to **Settings → Pages**.
4. Under *Source*, choose the `main` branch and the `/ (root)` folder, then save.
5. Your site will be live at `https://your-username.github.io/repository-name` within a minute or two.

### Option B: Netlify (drag and drop)

1. Go to [netlify.com](https://www.netlify.com) and sign in.
2. Drag your project folder onto the deploy area.
3. Netlify gives you a live link instantly, and you can set a custom name.

### Option C: Vercel

1. Push the project to GitHub.
2. Import the repository on [vercel.com](https://vercel.com).
3. Click **Deploy**.

---

## 🌐 Browser Support

Works in the latest versions of **Chrome, Edge, Firefox and Safari**, on desktop and mobile.

---

## 🗺️ Roadmap

- [ ] Add real project screenshots
- [ ] Connect the contact form to a service (Formspree or EmailJS) so messages send without opening an email app
- [ ] Add a downloadable resume button
- [ ] Add a blog or "Learning log" section
- [ ] Add my Smart India Hackathon project once it is done

---

## 🧠 What I Learned

- Building a **multi-page site without a framework** using hash-based routing
- Rendering UI from **JavaScript data** instead of repeating HTML
- CSS **animations, glassmorphism and theming** with variables
- Drawing animated graphics with the **Canvas API**
- Handling **forms, validation and events** in the DOM

---

## 🤝 Feedback

Found a bug or have a suggestion? Open an issue or send a message through the Contact page.

## 📄 License

This project is open source under the [MIT License](LICENSE). You are free to use it as a template for your own portfolio. A star ⭐ or a credit is always appreciated.

---

<div align="center">

**Built with ❤️ by [Vihaan Khanna](https://github.com/your-username)**
First-year CSE (AI/ML) student · Learning, building, shipping

</div>
