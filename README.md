# HANGZHOU KUVO IMPORT AND EXPORT CO., LTD. — Website

A complete Create React App rebrand for KUVO, using the supplied product photographs and a new navy/gold corporate identity.

## Included
- Responsive homepage, About, Products, product detail pages, Markets, FAQ, Insights and Contact/Quote form
- KUVO logo and favicon; all former Guangdong Energy brand references removed
- Supplied image archive integrated into `public/assets/products/`
- English/Chinese interface switch (navigation and selected homepage/product labels)
- SEO titles/descriptions, Open Graph metadata, Organization structured data, sitemap and robots.txt
- Product quotation inquiries with a product prefilled from product pages
- EmailJS-ready form with a mailto fallback if EmailJS is not configured

## Requirements
- Node.js 18 or 20 recommended
- npm

## Run locally
```bash
npm install
npm start
```
The development server opens at http://localhost:3000.

## Build for production
```bash
npm run build
```
The optimized static website is generated in `build/`.

## Set up direct inquiry email (recommended)
The inquiry form can send directly through EmailJS after you configure your own service, template and public key. The website package does not contain private EmailJS credentials.

1. Create an EmailJS account and connect the mailbox you want to receive inquiries at (currently configured recipient: `HANGZHOUKUVO@yahoo.com`).
2. Create an email template. Suggested template variables: `{{from_name}}`, `{{company}}`, `{{reply_to}}`, `{{country}}`, `{{product}}`, `{{quantity}}`, `{{message}}`, `{{to_email}}`.
3. Copy `.env.example` to `.env` in the project root.
4. Replace the three placeholder values with your EmailJS Service ID, Template ID and Public Key.
5. Restart `npm start` or rebuild after setting environment variables.

If EmailJS is not configured, submitting the form prepares a message in the visitor's default email application addressed to `HANGZHOUKUVO@yahoo.com`. A mail application must be installed/configured for that fallback.

## Company details currently used
- Company: HANGZHOU KUVO IMPORT AND EXPORT CO., LTD.
- Address: Room 1902-05, Building 10, Yuncuixuan, Liangzhu Street, Yuhang District, Hangzhou City, Zhejiang Province, China
- Website: https://www.hangzhoukuvo.com
- Sales email: HANGZHOUKUVO@yahoo.com
- Business email: not provided yet

## Before publishing
- Confirm the company address formatting and official English/Chinese legal name.
- Confirm all merchandise categories, product specifications, supplier permissions and product images.
- Add a business email/phone/WhatsApp if available.
- Configure EmailJS, test an inquiry end-to-end and set domain/DNS hosting.
- Replace editorial insight cards with approved articles before presenting them as published company news.
- Confirm privacy policy and terms appropriate to the company's jurisdiction and markets.

## Project structure
- `src/Pages/` — page components
- `src/Components/` — navigation and footer
- `src/assets/products.js` — editable product category catalogue
- `public/assets/products/` — website product imagery
- `public/brand/` — KUVO logo and favicon
