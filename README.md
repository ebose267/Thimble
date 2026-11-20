# Thimble — Front-end website

A responsive, single-page Thimble website built with plain HTML, CSS and JavaScript. There are no framework, package-manager or build-step requirements.

## Run it

Open `index.html` in a browser. For a local development server, open this folder in VS Code and use the Live Server extension, or run any simple static-file server.

## Brand direction used

The implementation follows the supplied Thimble mood board:

- Onyx: `#111111`
- Snow: `#FAFAF8`
- Amber: `#EFCB45`
- Mist: `#E8E6EB`
- Slate: `#6B6B6B`
- Poppins typography
- Lowercase `thimble.` wordmark with the amber full stop
- The three stated capabilities: Web Development, Business Automation and Digital Infrastructure
- The stated brand principles: Precision, Innovation, Reliability and Impact
- Brand line: “Thoughtfully engineered digital experiences.”

## Add the Cloudinary images

Open `script.js` and replace the empty strings in the `CLOUDINARY` object with the actual HTTPS Cloudinary delivery URLs. The image frames are already sized, cropped and responsive.

```js
const CLOUDINARY = {
  hero: "https://res.cloudinary.com/YOUR_CLOUD/image/upload/...",
  architecture: "https://res.cloudinary.com/YOUR_CLOUD/image/upload/...",
  detail: "https://res.cloudinary.com/YOUR_CLOUD/image/upload/..."
};
```

The three reserved slots are:

- `hero`: the real Thimble / thimble-object photograph.
- `architecture`: the architectural photograph in the dark visual section.
- `detail`: the architectural detail photograph in the lower image panel.

Use the original image URLs supplied for Thimble. No generated or stock photographs are bundled with this front end. Until URLs are added, the frames display restrained CSS-only compositions rather than invented photographs.

## Connect the enquiry form

In `script.js`, set:

```js
const CONTACT_EMAIL = "the-real-inbox@example.com";
```

The form then opens the visitor's email application with the enquiry prefilled. It does not store data or send anything to a server. For a production form that submits without opening an email app, connect a real backend or form service before launch.

## Before publishing

1. Add the final Cloudinary image URLs.
2. Add the real contact email or connect a real form endpoint.
3. Confirm the final service descriptions and contact wording.
4. Test on a phone and desktop, including the mobile navigation and contact form.
5. Confirm the correct legal, privacy and business information before adding it to the footer.

## Files

- `index.html` — page content and structure.
- `styles.css` — layout, responsive styling, brand system and motion.
- `script.js` — image slots, mobile navigation, reveal effects and email form behaviour.
