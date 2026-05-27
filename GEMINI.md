# Project Overview: Lucky Mystery Scoops (Shopify Theme)

This project is a custom Shopify theme for "Lucky Mystery Scoops," a retail concept centered around mystery scoops of charms and treasures. The website features a dual-theme design narrative ("Kuromi" for dark/mischievous and "My Melody" for light/sweet), bridging "mischievous gothic" and "soft sweetness."

## Core Technologies
- **Frontend:** HTML5, Vanilla CSS3 (utilizing Glassmorphism and Tactile Modernism).
- **Templating:** Shopify Liquid.
- **Platform:** Shopify.

## Directory Structure
- `assets/`: Contains project-wide SVG icons, package imagery, and the main stylesheet (`style.css`).
    - `Paket 1.png` to `Paket 4.png`: Mystery scoop package representations.
    - `style.css`: Comprehensive styling for the dual-theme experience.
- `layout/`: Contains the base theme layout.
    - `theme.liquid`: The master layout file handling the header, footer, and global asset loading.
- `templates/`: Shopify-specific page templates.
    - `index.liquid`: Main landing page with Kuromi and My Melody sections.
    - `cart.liquid`: Custom cart experience for reviewing and managing scoops.
    - `product.liquid`: Individual product detail template.
    - `page.about.liquid`: "About Us" page template.
    - `page.contact.liquid`: "Contact Us" page template with Shopify's contact form integration.
- `config/`: Configuration files for the theme settings.
- `locales/`, `sections/`, `snippets/`: Standard Shopify theme directories (currently placeholders for expansion).

## Design Conventions
- **Themes:**
    - **Kuromi (Night-Mode):** Deep purple gradients, high-saturation pink accents, glassmorphism (background-blur). Implemented via a fixed background gradient on `body`.
    - **My Melody (Day-Mode):** Pastel pinks, pure white surfaces, soft ambient shadows.
- **Asset Referencing:** All assets must be referenced using Liquid filters:
    - Images: `{{ 'filename.png' | asset_url }}`
    - Stylesheets: `{{ 'style.css' | asset_url | stylesheet_tag }}`
- **Typography:**
    - **Headlines:** Spline Sans (Bold/Black).
    - **Body/UI:** Plus Jakarta Sans.

## Building and Running
This project is managed using the [Shopify CLI](https://shopify.dev/themes/tools/cli).

- **Development:** To preview the theme locally on a Shopify store:
  ```bash
  shopify theme dev
  ```
- **Deployment:** To push changes to your Shopify store:
  ```bash
  shopify theme push
  ```
- **Linting:** To check for Liquid best practices and errors:
  ```bash
  shopify theme check
  ```

## Contribution Guidelines
- Adhere strictly to the color palettes and typographic scales.
- Ensure all new templates or sections follow the existing Glassmorphism and Tactile Modernism styles.
- Maintain the "Sparkle" motif through micro-interactions and decorative elements.
- Use Shopify Liquid filters for all dynamic content and asset loading.
