LaptopWorker - static HTML version
==================================

Upload the CONTENTS of this folder (including the hidden .htaccess file) to the web root of
laptopworker.com, or to any subfolder for a staging preview. All links are relative.

All 99 URLs are unchanged (home, blog, contact-us, cart, 31 posts, the extra theme pages,
categories, author pages, paginated pages and image attachment pages).
Each URL is a folder containing index.html.

Contact form
------------
Contact Form 7 needed WordPress, so the form now posts to contact-us/send.php (needs PHP).
IMPORTANT: open contact-us/send.php and set $to to the address that should receive messages.
Until then the form shows its error message instead of sending.

Noindex (staging)
-----------------
Every page has <meta name="robots" content="noindex, nofollow" /> and .htaccess sends an
X-Robots-Tag: noindex, nofollow header, so search engines will not index this copy.
BEFORE GOING LIVE on the real domain: remove that meta line from each page and delete the
"BEGIN noindex ... END noindex" block from .htaccess, or the site will drop out of Google.

Notes
-----
- /cart/ is a WooCommerce page; as static HTML it shows the page layout only (no shopping cart).
- The "related posts" box shows a fixed set of posts instead of a random set on each visit.
- The images for "Quote of the Day - The Power of Thought" are already missing on the live site.
