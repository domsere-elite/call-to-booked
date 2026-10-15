# Copperline site

Single-file static site for the Revenue Capture offer: `index.html` (inline CSS and JS, Google Fonts only) plus `og.jpg` for link previews. No build step. Open `index.html` in a browser, or serve the folder from any static host.

On GitHub Pages it lives at `/call-to-booked/site/`, next to the SVGator template page at the repo root, which is left untouched.

## Before it goes live

Search `index.html` for `TODO(Dom)`. Each one is a decision or a detail only you can fill in:

| What | Where |
| --- | --- |
| Form endpoint (GHL inbound webhook, Formspree, etc.) | `CONFIG.formEndpoint` in the script. While it's empty the form shows success but **sends nothing**. |
| Audit booking link (GHL calendar or Cal.com) | `CONFIG.calendarUrl`. Empty hides the "Book a 15-minute call" button. |
| Phone number and email | Footer, Contact column |
| Business legal name | Footer copyright line |
| Guarantee in or out | Pricing, the `.guar` block |
| Month-to-month vs. 3-month minimum | Pricing terms line and the "Is there a contract?" FAQ |
| Website add-on price ("From $1,500" is a placeholder) | Pricing, website add-on |
| Final domain | `og:image` and `og:url` meta tags |

The form posts JSON: `name`, `business`, `phone`, `trade`, `website_interest`, `source`, `page`, `submitted_at`.

## Renaming

"Copperline" is plain text. Find-and-replace it across `index.html`. The logo mark is a drawn shape, so it doesn't need to change. Regenerate `og.jpg` afterwards (it's a screenshot of the hero).

## Sample content

The call transcript, text threads, monthly report and review are illustrations. "Hartwell Air & Plumbing" is a made-up shop, and every sample is labeled as a sample on the page. The 80% and 78% figures come from the business brief; have a source ready in case a prospect asks.
