# Sinii Kira — Enterprise E-Commerce Financial Intelligence Suite

**Sinii Kira** (`www.sinii.my`) is a high-performance, enterprise-grade e-commerce financial auditing and take-home margin intelligence application designed specifically for Malaysian online sellers. It provides real-time fee comparisons, reseller/agent commission breakdowns, SST (8%) adjustments, and break-even pricing calculations across major marketplace platforms.

## 🚀 Key Features

* **Multi-Platform Fee Audit**:
  * **Shopee**: Category commissions, payment gateway transaction fees (including SPayLater), platform support fees (RM0.50 + SST), and optional Cashback/Free Shipping program fees.
  * **TikTok Shop**: Marketplace commissions, TikTok PayLater transaction fees, and extra platform support fees.
  * **Lazada**: Category commission rates and updated payment fees (3.5% + SST).
  * **PGMall**: Flat seller commission and payment processing fee structure.
  * **Own Website / Custom Gateway**: Configurable FPX/Card gateway percentages (Billplz, Stripe, ToyyibPay) plus fixed per-transaction charges.
  * **Sinii Platform**: Planned ecosystem model preview.

* **Reseller & Affiliate Calculations**:
  * Deducts agent/dropship commission percentages and affiliate commission payouts directly from net profit calculations.

* **Target Margin Reverse-Engineer**:
  * Input your desired net margin percentage (e.g., 30%) and instantly compute the minimum selling price needed per platform.

* **Enterprise Audit Engine**:
  * Export clean, audit-ready financial summaries to clipboard or printable PDF via custom `@media print` stylesheets.

* **100% Privacy & PDPA 2010 Compliant**:
  * Operates entirely **client-side** in the user's browser. Zero server data logging, ensuring sensitive COGS and profit data never leak.

* **Single-File Architecture**:
  * Zero build steps or Node.js dependencies required; runs out-of-the-box using HTML5, Vanilla JS, and Tailwind CSS CDN.

## 📂 Repository Structure

```
.
├── index.html       # Primary application entry point (UI + Logic)
├── _headers         # Cloudflare Pages security & caching header policies
├── DEPLOYMENT.md    # Detailed guide for Cloudflare Pages & DNS setup
└── README.md        # Project documentation
```

## ⚡ Quick Start / Local Development

Since **Sinii Kira** is built as a lightweight single-file web application, you can run it locally without any build toolchain:

1. **Clone or Download the Repository**:
   ```bash
   git clone https://github.com/khaliffhaned-dot/sinii.git
   cd sinii
   ```

2. **Open directly in a Browser**:
   * Double click `index.html` or open it directly in Chrome, Firefox, Safari, or Edge.

3. **Or run with a local HTTP server** (e.g., Python / Node):
   ```bash
   # Using Python 3
   python3 -m http.server 8000
   
   # Or using npx
   npx serve .
   ```
   Navigate to `http://localhost:8000`.

## ☁️ Onboarding & Cloudflare Deployment

For full deployment instructions, custom domain routing (`sinii.my`), and DNS configuration for Namecheap PrivateEmail (`admin@sinii.my`), refer to the included [**DEPLOYMENT.md**](./DEPLOYMENT.md) guide.

### Fast Cloudflare Pages Deploy

1. Push this repository to GitHub (`khaliffhaned-dot/sinii`).
2. In Cloudflare Dashboard, go to **Workers & Pages** → **Create Application** → **Pages**.
3. Select your `khaliffhaned-dot/sinii` repository, set the build output directory to `/`, and click **Deploy**.
4. Add custom domains `sinii.my` and `www.sinii.my` under the project settings.

## ⚖️ Legal & Compliance Notice

* **Malaysian Consumer Protection Act 1999 & Sales Tax Act 2018**:
  All platform fee calculations factor in standard 8% Sales and Service Tax (SST) rules applicable to digital services in Malaysia.

* **Personal Data Protection Act 2010 (PDPA)**:
  All processing occurs locally in the user's browser environment.

* **Third-Party Trademarks**:
  Shopee, TikTok Shop, Lazada, and PGMall are registered trademarks of their respective owners. Sinii Kira is an independent software tool operated by **Sinii Malaysia** (`www.sinii.my`).

## 📩 Support & Contact

* **Website**: [www.sinii.my](https://www.sinii.my)
* **Official Admin Email**: [admin@sinii.my](mailto:admin@sinii.my)
* **License**: Proprietary / All Rights Reserved © 2026 Sinii Malaysia.