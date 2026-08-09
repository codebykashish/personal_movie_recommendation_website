# 🎬📚 Personal Movie & Book Archive
### *A MERN Stack Learning Journey*

> A personal, artistic digital archive of everything I've watched and read — built as a project-driven path into the MERN stack.

---

## ✨ Project Overview

This isn't just another movie database. It's a reflection of **personal taste** — movies and books I've experienced, my ratings, my reviews, my favorites, and curated *"must-watch / must-read"* lists.

The visual direction is **Pinterest-inspired**: artistic, cute, typography-forward, image-rich, and full of small delightful animations.

The technology is a vehicle for learning — I'll pick up each MERN concept exactly when the project needs it, rather than studying everything in isolation first.

| 🎯 Goal | Understand how a complete full-stack app works — from click to database and back |
|---|---|
| 🧠 Method | Project-driven learning — learn a concept only when a feature needs it |
| 🎨 Style | Editorial, scrapbook-like, cinematic, cozy-curated |

---

## 🏗️ Final Architecture

| Layer | Technology |
|---|---|
| 🎨 Frontend | **React** |
| 🖥️ Runtime | **Node.js** |
| 🔌 API Layer | **Express.js** |
| 🗄️ Database | **MongoDB** |
| 🧬 Modeling | **Mongoose** |
| 🔐 Access Control | **Authentication** |
| 🔧 Workflow | **Git / GitHub** |

---

## 🗺️ The Roadmap

```
Phase 0 → Foundations
Phase 1 → Frontend Prototype
Phase 2 → Backend & API
Phase 3 → MongoDB Database
Phase 4 → Authentication & Admin
Phase 5 → Advanced Features
Phase 6 → UI/UX Refinement
Phase 7 → Deployment
```

---

## 🧱 Phase 0 — Foundations

*Before React, lock in the fundamentals.*

<details>
<summary><strong>📋 Topics to learn</strong></summary>

**HTML & CSS**
- Semantic structure
- Flexbox & Grid
- Positioning
- Responsive design
- Typography & visual hierarchy

**JavaScript**
- Syntax, variables, data types
- Functions, conditions, loops
- Arrays, objects
- `map()`, `filter()`, `find()`, `sort()`
- Destructuring & spread syntax
- Modules — `import` / `export`
- JSON
- DOM & event handling
- Promises & `async/await`
- `fetch()` and HTTP basics

**Tooling**
- Git & GitHub fundamentals

</details>

> 💡 The goal isn't mastery — just enough to start building, then deepen as needed.

---

## 🎨 Phase 1 — Frontend Prototype

*The visual identity and UX come first. No backend yet — just local JS/JSON data.*

**Stack:** React · JavaScript · HTML · CSS · React Router · Git/GitHub

### 🧭 Site Map

| Page | Purpose |
|---|---|
| 🏠 Home | Landing + curated highlights |
| 🎞️ Movies | Full movie collection |
| 📖 Books | Full book collection |
| 🏆 Top 10 / Must-Watch | Curated favorites |
| ⭐ Favorites | Personal picks |
| 🎯 Recommendations | For visitors |
| 🔍 Detail Pages | Individual movie/book view |
| 💭 About / My Taste | Personal statement |

### 🏠 Homepage Sections

- 💌 Introduction / personal statement
- 🔥 Currently obsessed with
- 🏆 Top 10 recommendations
- 🕓 Recently watched
- ❤️ Favorite movies
- 📚 Favorite books
- 🎁 Curated recommendations
- 🎲 "Pick something for me"

### ⚛️ React Concepts

`Components` · `Props` · `State` · `Event Handling` · `Conditional Rendering` · `Rendering Lists` · `Forms` · `useState` · `useEffect` · `React Router` · `Component Composition`

> 🧩 Example: a reusable `<MovieCard />` component takes movie data as props and renders the title, poster, rating, and genre.

### ✅ Feature Checklist

- [ ] Movie cards
- [ ] Book cards
- [ ] Detail pages
- [ ] Search
- [ ] Filter by genre/category
- [ ] Sort by rating/year/title
- [ ] Mark favorites
- [ ] Curated Top 10 lists
- [ ] Responsive layout
- [ ] Basic animations

> 🎯 **North star for Phase 1:** it should feel like a real personal product, not a tutorial project.

---

## ⚙️ Phase 2 — Backend & API

*Manually editing JS files to add a movie doesn't scale. Time for a real backend.*

**Stack:** Node.js · Express.js · REST API · MongoDB · Mongoose

### 📘 Concepts

Node fundamentals · npm & packages · Express server · HTTP methods · REST architecture · Routes · Request/Response objects · Middleware · Status codes · Error handling · Environment variables · Database connections

### 🔌 Initial API Design

**🎞️ Movies**
```
GET     /api/movies
GET     /api/movies/:id
POST    /api/movies
PUT     /api/movies/:id
DELETE  /api/movies/:id
```

**📖 Books**
```
GET     /api/books
GET     /api/books/:id
POST    /api/books
PUT     /api/books/:id
DELETE  /api/books/:id
```

---

## 🗄️ Phase 3 — MongoDB Database

*Persistent storage replaces hardcoded data.*

### 📦 Collections

`Movies` · `Books` · `Users` · `Reviews` · `Tags`

<table>
<tr>
<th>🎞️ Movie Document</th>
<th>📖 Book Document</th>
</tr>
<tr>
<td>

```
title
year
genres
poster
rating
review
favorite
watchedDate
tags
recommendationLevel
```

</td>
<td>

```
title
author
cover
rating
review
favorite
finishedDate
genres
tags
```

</td>
</tr>
</table>

### 📘 Concepts

Databases · Collections · Documents · CRUD · MongoDB queries · ObjectId · Mongoose schemas & models · References · Validation · Basic indexing

### 🔄 Full Data Flow

```
       React
         ↓
   HTTP Request
         ↓
   Express API
         ↓
      Node.js
         ↓
     MongoDB
         ↓
    Response
         ↓
     React UI
```

---

## 🔐 Phase 4 — Authentication & Admin System

*Public browsing stays open. Editing stays private.*

```
                 🌐 Website
                    │
          ┌─────────┴─────────┐
          ↓                   ↓
      👀 Visitors          🔑 Owner
          ↓                   ↓
    View content        Login / Admin
                              ↓
                    Add / Edit / Delete
```

### ✨ Features

- User registration/login
- Password hashing
- Protected API routes
- Login/logout
- Admin dashboard → Add · Edit · Delete movies & books

### 📘 Concepts

Authentication vs. authorization · Password hashing · Cookies/tokens · Protected routes · Auth middleware · Secure env variables · Basic web security

---

## 🚀 Phase 5 — Advanced Features

*Once the core app works — layer on the fun stuff.*

### 🔍 Advanced Search
`Title` · `Author` · `Genre` · `Tag` · `Year` · `Rating`

### 🎛️ Filtering Example
```
Genre:     Drama
Rating:    4+
Year:      2010–2026
Favorite:  Yes
```

### 🧠 Recommendation Engine (rule-based, v1)
```
IF genre = psychological AND rating >= 4
→ display highly rated items with matching tags
```
> *(Could evolve into something smarter later — only if there's a real reason to.)*

### 🎲 "What Should I Watch?"
A button that randomly surfaces something from the curated collection.

### 📊 Personal Stats Dashboard

| Metric | Tracked |
|---|---|
| 🎞️ Total movies watched | ✅ |
| 📚 Total books read | ✅ |
| ⭐ Average rating | ✅ |
| 🎭 Favorite genres | ✅ |
| 📅 Most-watched years | ✅ |
| 🕓 Watching/reading history | ✅ |
| 🎁 Number of recommendations | ✅ |

### 🌱 Future Possibilities

- 🖼️ Image uploads
- 🌐 External movie/book API integration
- 📌 Watch/read status + watchlist
- 🌙 Mood-based recommendations
- 📝 Notes & quotes
- 🕰️ Reading/watching timeline
- 🔗 Shareable recommendation pages

---

## 🎨 Phase 6 — UI/UX & Visual Refinement

*Design isn't an afterthought — it's core to the product.*

**Inspiration:** Pinterest · Digital scrapbooks · Personal journals · Cinematic aesthetics · Editorial layouts

| Focus Area | Details |
|---|---|
| 🔤 Typography | Voice & hierarchy |
| 🎨 Color palette | Mood-setting |
| 🃏 Card design | Signature look |
| 🧱 Layout | Masonry / grid |
| 🌬️ Whitespace | Breathing room |
| 📱 Responsive design | Mobile-first feel |
| ✨ Micro-interactions | Hover effects, transitions |
| 🖼️ Image treatment | Consistent visual language |
| 🎀 Decorative elements | Personality touches |

> 🎯 The end result should feel like a **curated creative space**, not a database interface.

---

## 🚢 Phase 7 — Deployment & Production

*Time to make it live.*

### 📘 Topics
Production builds · Environment variables · Frontend & backend deployment · Database hosting · CORS · Production API config · Basic security · Git/GitHub workflow · Error monitoring

### 🏛️ Final Architecture

```
            👤 USER
              ↓
       ⚛️ React Frontend
              ↓
         🔌 REST API
              ↓
     🖥️ Express + Node
              ↓
         🗄️ MongoDB
```

---

## 🧭 Overall Learning Strategy

> **Project-first, always.** Learn only what the next feature demands.

```
Learn JS fundamentals
        ↓
Build small frontend features
        ↓
Learn React
        ↓
Build the visual website
        ↓
Need dynamic data → Learn Node + Express
        ↓
Build REST API
        ↓
Need persistent storage → Learn MongoDB
        ↓
Connect database
        ↓
Need private content mgmt → Learn authentication
        ↓
Build admin system
        ↓
Need better functionality → Add advanced features
        ↓
🚀 Deploy the complete MERN application
```

### 🎓 Skills Developed

`JavaScript` `React` `Node.js` `Express` `MongoDB` `REST APIs` `Authentication` `Databases` `Git` `UI/UX` `Software Architecture` `Deployment`

---

## 🏁 Final Goal

> A **personal, artistic** movie & book archive — shareable with anyone who asks *"what should I watch/read?"*

Visitors explore watched movies, read books, personal ratings, reviews, favorites, and curated Top 10s. The owner gets a private admin space to manage it all.

Beyond the product itself, this project doubles as a **substantial portfolio piece** — proof of both frontend creativity and full-stack engineering skill.

> 🌱 *The project starts small and evolves. Advanced features only get added when they earn their place.*