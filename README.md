# CLAYCHARMS — Bespoke Handcrafted Clay Charms & Keepsakes

[![License: MIT](https://img.shields.io/badge/License-MIT-C5A059.svg)](LICENSE)
[![Status: Production Ready](https://img.shields.io/badge/Status-Marketplace--Ready-10B981.svg)]()
[![Theme: Luxury Dark](https://img.shields.io/badge/Theme-Dark%20%26%20Champagne%20Gold-C5A059.svg)]()

> **CLAYCHARMS** is a high-end, responsive e-commerce showcase built for made-to-order handcrafted polymer clay jewelry, artisan charms, custom pendants, and bespoke keepsakes.

---

## ✨ Features & Architecture

### 1. Direct WhatsApp Commerce Gateway
- **Zero Friction Checkout:** Customers curate their bag, input custom requirements (colors, initials, specific dimensions), and click **"Buy Now via WhatsApp"**.
- **Automated Message Dispatch:** The cart automatically compiles chosen pieces, quantities, and notes into an organized pre-formatted message sent directly to the creator's WhatsApp (`+91 7702735531`):
  ```text
  *NEW ORDER INQUIRY — CLAYCHARMS* 🛍️

  Hello! I would like to place an order for the following custom handcrafted pieces:
  1. *Artisan Clay Pendant No. 01* — Quantity: 1
  2. *Sculpted Clay Charm No. 02* — Quantity: 2

  *Customer Customization Note:* "Personalized gold lettering"

  Please let me know the pricing quotation, crafting timeframe, and payment instructions. Thank you!
  ```
- **Instant Single-Piece Orders:** Every product card also features an instant "Buy via WhatsApp" button for quick 1-tap inquiries.
- **Floating Concierge:** Compact, non-intrusive floating WhatsApp action button in the bottom-right for instant consultation.

---

### 2. Ultra-Luxury Minimalist Aesthetic
- **Color Palette:**
  - **Backgrounds:** Deep rich blacks & charcoals (`#0A0A0A`, `#121212`, `#161616`)
  - **Primary Brand Accent:** Champagne Gold (`#C5A059`) with polished gold hover highlights (`#D4AF37`)
  - **Typography:** Softened luxury cream headings (`#F8F4E6`) avoiding stark harsh whites
  - **Borders & Dividers:** Subtle metallic low-opacity gold glows (`border-[#C5A059]/20`)
- **Artisan Typography:** Hand-paired pairing of *Cormorant Garamond* (editorial serif titles) and *Inter* (crisp technical sans-serif).
- **Subtle Film Grain Texture:** Subtle background noise overlay giving a tactile handcrafted feel.

---

### 3. Curated 12-Piece Product Catalogue
Structured with category filtering (All, Charms, Pendants, Keepsakes) and precise piece numbering:

| Piece | Item Name | Category | Primary Asset |
| :---: | :--- | :---: | :--- |
| **#01** | Artisan Clay Pendant No. 01 | Pendants | `images/product-07.jpg` |
| **#02** | Sculpted Clay Charm No. 02 | Charms | `images/product-06.jpg` |
| **#03** | Sculpted Clay Charm No. 03 | Charms | `images/product-04.jpg` |
| **#04** | Bespoke Clay Keepsake No. 04 | Keepsakes | `images/product-05.jpg` |
| **#05** | Sculpted Clay Charm No. 05 | Charms | `images/product-02.jpg` |
| **#06** | Sculpted Clay Charm No. 06 | Charms | `images/product-01.jpg` |
| **#07** | Bespoke Clay Keepsake No. 07 | Keepsakes | `images/product-08.jpg` |
| **#08** | Sculpted Clay Charm No. 08 | Charms | `images/product-09.jpg` |
| **#09** | Artisan Clay Pendant No. 09 | Pendants | `images/product-10.jpg` |
| **#10** | Sculpted Clay Charm No. 10 | Charms | `images/product-11.jpg` |
| **#11** | Bespoke Clay Keepsake No. 11 | Keepsakes | `images/product-12.jpg` |
| **#12** | Sculpted Clay Charm No. 12 | Charms | `images/product-13.jpg` |

---

### 4. Responsive Mobile Optimization
- **2-Column Mobile Luxury Grid (`grid-cols-2`):** Modern high-fashion mobile storefront browsing (mirroring SSENSE / Zara mobile standards).
- **Dedicated Touch Quick-Action CTAs:** Mobile view displays clean touch buttons (`+ Bag` and `WhatsApp`) directly under product details, while desktop retains elegant hover overlays.
- **Zero Horizontal Overflow:** Strict viewport-clamping (`max-w-full`, `overflow-x-hidden`) ensures no side-scrolling, clipping, or viewport shaking on any iPhone or Android screen width.
- **Full Slide-Over Bag Drawer:** Responsive mobile slide-over cart with backdrop blur and touch dismiss.

---

### 5. High-Speed Performance & Core Web Vitals
- **Resource Hints:** `dns-prefetch` and `preconnect` established for Google Fonts and Tailwind CDN.
- **Hero Image Preload:** Critical Largest Contentful Paint (LCP) hero asset preloaded via `<link rel="preload">` with `fetchpriority="high"`.
- **Native Lazy Loading:** All below-the-fold catalog images utilize `loading="lazy"` and `decoding="async"`.
- **Layout Stability:** Explicit aspect ratios and image dimensions prevent Cumulative Layout Shift (CLS = 0).
- **CSS Content Visibility:** `content-visibility: auto` applied to off-screen sections (`#catalog`, `#craftsmanship`, `#contact`, `#footer`) to defer initial paint and layout computation.
- **Hardware Acceleration:** Smooth hover transitions powered by GPU `will-change: transform`.

---

### 6. Technical SEO & Schema.org Structured Data
- **Metadata:** Targeted title (57 chars), compelling meta description (153 chars), and relevant long-tail keywords.
- **Open Graph & Twitter Cards:** Complete rich sharing cards configured for WhatsApp, iMessage, Instagram, Facebook, and Twitter.
- **JSON-LD Schema Markup:** Integrated Schema.org `Store` / `LocalBusiness` data with catalog categorization, currency (`INR`), and WhatsApp order gateway information for Google Rich Search Results.
- **Descriptive Image Alt Tags:** Every product image contains keyword-rich semantic descriptors optimized for Google Image Search.

---

## 🚀 How to Run Locally

Because the project is built with standard HTML, Tailwind CSS (via CDN), and vanilla JavaScript, no build step or package installation is required:

```bash
# Clone the repository
git clone https://github.com/manishbollikonda-318/CLAYCHARMS.git

# Navigate into the project directory
cd CLAYCHARMS

# Start any local HTTP server (e.g. with Python 3)
python3 -m http.server 8080
```
Open [http://localhost:8080](http://localhost:8080) in your browser.

---

## 🌐 Deploy to GitHub Pages (1-Click)

1. In your GitHub repository, go to **Settings** > **Pages**.
2. Under **Build and deployment** > **Source**, select **Deploy from a branch**.
3. Choose the **`main`** branch and root **`/ (root)`** folder, then click **Save**.
4. Your website will be live in seconds at:
   `https://manishbollikonda-318.github.io/CLAYCHARMS/`

---

## 🛠️ Tech Stack
- **Structure:** Semantic HTML5
- **Styling:** Tailwind CSS v3 with customized luxury theme extension
- **Typography:** Cormorant Garamond + Inter (Google Fonts)
- **Icons:** Inline lightweight SVGs
- **Data & Cart:** Vanilla JavaScript (ES6+, zero runtime dependencies)
- **Deployment:** GitHub Pages / Vercel / Netlify ready

---

## 📄 License
This project is licensed under the [MIT License](LICENSE).
