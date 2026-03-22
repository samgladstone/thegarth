# The Garth

## Problem Statement

The owner of The Garth — a 3-bedroom holiday cottage in Gunnerside, Swaledale — currently takes all bookings via AirBnB. They want to capture direct bookings to reduce platform dependency and fees. A simple website is needed to establish a direct online presence, surface the property in local search results, and funnel interested guests to contact via WhatsApp.

## Target Users

- Prospective holiday guests searching for short-term rentals in Swaledale / the Yorkshire Dales
- Guests who have heard of The Garth by word of mouth and want to find contact details

## Key Use Cases

1. A guest searches "holiday cottage Gunnerside" and finds the site via Google
2. A guest lands on the site and gets a clear sense of the property (location, size, feel)
3. A guest initiates a booking enquiry via WhatsApp
4. A guest who prefers AirBnB is directed there to book

## Constraints

- Content sourced from the AirBnB listing; owner may supplement with additional detail/photos
- WhatsApp is the sole direct contact method
- Site must be maintainable by the developer with minimal ongoing effort
- Hosting must be low/no cost (Vercel free tier)
- No CMS — content is managed via code

## Success Metrics

- The following searches appear on the first page of Google results:
  - Holiday Cottage Gunnerside
  - Holiday Stay Swaledale
  - The Garth Gunnerside
  - The Garth
- 10% of bookings come directly (via WhatsApp), rather than via AirBnB

## Scope

### In Scope
- Single-page marketing website
- Property overview (description, photos, key details)
- WhatsApp CTA
- AirBnB listing link
- Google Maps link
- SEO fundamentals (meta tags, semantic HTML, structured data)
- Deployment to Vercel

### Out of Scope
- Availability calendar / AirBnB sync
- Online payment or booking forms
- CMS or admin interface
- Multi-page site structure
- Analytics beyond basic Vercel analytics

## Key Links

- [AirBnB Listing](https://airbnb.co.uk/h/thegarth)
- [WhatsApp Contact](https://wa.me/+447757250718)
- Domain: `thegarthgunnerside.co.uk`

---

## Getting Started

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start local dev server at `localhost:4321`  |
| `npm run build`   | Build for production to `./dist/`           |
| `npm run preview` | Preview production build locally            |
