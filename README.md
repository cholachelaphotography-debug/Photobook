# Chola Chela Photography — Photo Books Platform

A modern web application prototype for **Chola Chela Photography**, Zambia's dedicated photo book printing and design service.

## Vision

There is currently no dedicated local company in Zambia offering professional photo book printing and design services. This platform fills that gap by allowing clients to:

- Create accounts and log in securely (demo uses browser storage)
- Upload their photos
- Browse professionally designed templates
- Design custom photo books by placing photos into layout slots
- Prepare books for local printing and delivery

## Features (MVP Prototype)

- **Beautiful landing page** with branding, hero, features, and how-it-works
- **User accounts**: Sign up / Log in (data stored in browser localStorage for this demo)
- **Photo library**: Drag-and-drop or click-to-upload photos
- **Template gallery**: 6 curated templates (Classic Grid, Story Spread, Minimal, Wedding, Travel, Family)
- **Photo book editor**:
  - Multi-page books
  - Click slots to select, then click photos to place
  - Page navigation
  - Clear individual photos
  - Mark as ready for print
- **Responsive design** works on desktop and mobile
- **Local-first**: No external backend required for the demo

## How to Run

Simply open `index.html` in a modern browser, or serve the folder:

```bash
# Python
python3 -m http.server 8080

# Or Node
npx serve .
```

Then visit http://localhost:8080

## Tech Notes

- Pure client-side (HTML + React via CDN + Tailwind via CDN)
- No build step required
- All data (users, photos as base64, projects) persists in `localStorage`
- Suitable as a high-fidelity prototype / design reference

## Next Steps for Production

1. Real backend (Node/Next.js or Firebase) with proper authentication
2. Cloud image storage (S3, Cloudinary, or local server)
3. Advanced canvas editor (Fabric.js / Konva) for free-form design
4. Payment integration + order management
5. Print partner API or local production workflow
6. Admin dashboard for managing orders

---

Built for Chola Chela Photography · Lusaka, Zambia
