ORBIT WEBSITE
=============
Files: index.html, privacy.html, terms.html, legal.css, og-image.png, apple-touch-icon.png,
       favicon.svg, robots.txt, sitemap.xml

1) Put your real domain in (Termux, from inside this folder):
     sed -i 's#https://YOUR-DOMAIN.com#https://yourdomain.com#g' *.html robots.txt sitemap.xml

2) Replace the "Get Orbit" link. Search the three TODO comments in index.html
   (grep -n TODO index.html) and swap href="#" for your store / APK link.

3) Fill the yellow placeholders in privacy.html and terms.html
   (company name, contact emails, governing law, liability amount).
   Have a lawyer review both pages before launch.

4) Upload the whole folder to any static host (Netlify, Vercel, GitHub Pages, Cloudflare Pages).
   Keep og-image.png at the site root so link previews work.
