Deployment Report: Ecommerce Marketplace Builder

Project Overview

The Ecommerce Marketplace Builder is a full-stack eCommerce platform built using Next.js 15 on the frontend and Sanity CMS as the backend. The website allows users to browse products, manage carts, place orders, and track their purchases.

Project Links

Live Website: hackathon-4

GitHub Repository: hackathon-4 GitHub

Deployment on Vercel

Steps to Deploy on Vercel

Connect to GitHub:

Go to Vercel

Click on New Project and import the repository from GitHub.

Set Environment Variables:

In Vercel, navigate to Project Settings > Environment Variables.

Add the following local keys:

NEXT_PUBLIC_SANITY_PROJECT_ID: (Sanity Project ID)

NEXT_PUBLIC_SANITY_DATASET: (Dataset Name)

NEXT_PUBLIC_API_BASE_URL: (API Base URL)

NEXT_PUBLIC_STRIPE_KEY: (Stripe Payment Key)

Configure Build Settings:

Ensure that the build command is npm run build

Output directory remains default (.next)

Deploy the Project:

Click Deploy and wait for the process to complete.

Once deployed, Vercel provides a live URL.

Performance Optimization

Performance was tested using Web Test tools. Key improvements for better scores:

Image Optimization:

Used Next.js Image component for automatic optimizations.

Enabled lazy loading for faster page loads.

Code Splitting & Lazy Loading:

Implemented dynamic imports for components that are not immediately needed.

CSS & JavaScript Optimization:

Minified CSS & JS using built-in Next.js optimizations.

Removed unused CSS classes.

Server-Side Rendering (SSR) & Static Generation (SSG):

Used getServerSideProps and getStaticProps for better page rendering.

Caching & CDN:

Leveraged Vercel’s CDN for improved asset delivery.

Development Workflow

Tech Stack:

Frontend: Next.js 15 with TailwindCSS

Backend: Sanity CMS (Headless CMS)

Third-Party APIs:

Product Listings (/products)

Product Details (/products/{product_id})

Sanity API Endpoints:

Customer, Order, and Cart schemas

Payment Integration:

Easypaisa, JazzCash, Bank Transfer, and Stripe

Key Features Developed

User Authentication:

Users can sign up and log in using Google and GitHub.

Product Listings & Filters:

Fetched product data from third-party APIs.

Cart Management:

Implemented add/update/remove functionality using Context API.

Checkout Flow:

Integrated Sanity CMS to store orders and customer data.

Payment processing via multiple gateways.

Admin Panel:

Admins can manage orders, products, and inventory.

Conclusion

The Ecommerce Marketplace Builder was successfully deployed on Vercel with all necessary optimizations. The website achieves high performance and scalability while leveraging modern web technologies.

For further improvements, caching strategies and backend optimizations can be explored. 🚀


