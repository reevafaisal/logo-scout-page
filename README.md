# LogoScout

## Description
This project is a web-based image extraction tool that crawls websites and retrieves images efficiently, built primarily in Java. It is designed to extract images from a given URL, queue subpages within the same domain, and filter results for logos or other specific image types. The tool is optimized for performance and concurrency, ensuring that users receive results quickly while maintaining scalability.

## Key Features
- Supports any publicly accessible webpage as input.
- Handles missing or invalid URLs gracefully, providing test images as fallback.
- Uses JSoup to fetch and parse webpages for images.
- Queues subpages only within the same domain to prevent unnecessary external crawling.
- Implements multi-threaded crawling so that the crawl can be performed on multiple sub-pages at a time.
- Uses the Google Vision API to make image classification and to detect whether a logo is spotted within an image.
- All images produced link to respective page or sub-page that they have been crawled from.

---

### [Demo](https://web-production-ec8c.up.railway.app/)

  <p>
    <iframe src="https://prolific-elegance-production.up.railway.app/" width="100%" height="450" frameborder="0" scrolling="yes"></iframe>  
  </p>  

## Usage Instructions 

- Paste any public webpage url into the search bar ([test links provided below](./index.html#test-links)).
- Click any of the iamges produced to view the the specific webpage it has been crawled from.

## Test Links
- [https://jekyllrb.com/](https://jekyllrb.com/)
- [https://reevafaisal.github.io/Portfolio/](https://reevafaisal.github.io/Portfolio/)
- [https://www.simplyrecipes.com/our-most-popular-chicken-breast-recipe-11687586](https://www.simplyrecipes.com/our-most-popular-chicken-breast-recipe-11687586)
- [https://en.m.wikipedia.org/wiki/File:LEGO_logo.svg](https://en.m.wikipedia.org/wiki/File:LEGO_logo.svg)

---

Technologies: Java, JSoup, Gson, ExecutorService, HTML, CSS, JavaScript, JSON, Google Vision API
