<img src="./docs/component-images/hero-image.png" style="margin-bottom: 50px">

# <a id="top"></a> S.J. Smith Portfolio

Website: https://sjsmith.dev

Github: https://github.com/smith-sj/portfolio

## Table of Contents

- [Purpose](#purpose)
- [Target Audience](#target-audience)
- [Tech Stack](#tech-stack)
- [Functionality & Features](#functionality)
    - [Mobile First](#mobile-first)
    - [Responsive](#responsive)
    - [Accessibility](#accessibility)
- [Sitemap](#sitemap)
- [Screenshots](#screenshots)
- [Mobile](#mobile)
- [Desktop](#desktop)

---

## <a id="purpose"></a> Purpose

[[back to top]](#top)

The purpose of the project is to demonstrate my programming skills and experience to recruiters and potential employers. It is also an opportunity to show my personality and provide some insight into my creative process and personal aesthetic. Finally, it is an archive of articles for anyone who may be interested in web dev discussion, tutorials, and general news.

---

## <a id="target-audience"></a> Target Audience

[[back to top]](#top)

- Recruiters
- Employers
- Web dev enthusiasts

---

## <a id="tech-stack"></a> Tech Stack
[[back to top]](#top)
- HTML
- CSS
- JavaScript

* Repository hosted by GitHub
* Site deployed on Netlify

---

## <a id="functionality"></a> Functionality & Features

[[back to top]](#top)

The three main objectives I kept in mind while designing the functionality of my website were:

1. **Mobile First**
1. **Responsive**
1. **Accessible & Intuitive**

<a id="mobile-first"></a>

### Creating a mobile first website:

[[back to top]](#top)

This objective focused on designing the website from a **mobile user's perspective**, before making adjustments to suit tablet and desktop users. *Mobile first* isn't just about view-ports and layouts, but also involves consideration of the overall site map and functionality of each component. One of the first major decisions I made in this particular area, was to try and fit my important content on a single, well-organised and scroll-able page. I had already decided that my website would take a minimal approach to content, as I wanted the reader to quickly and easily understand my skills, interests and personality, without being overwhelmed with information.
<img align="left" style="margin: 20px" width="300" height="auto" src="./docs/component-images/accordian.png">

My solution to fitting all of this content on the homepage was to build these accordion-like content boxes. To build them, I used the HTML `<details>` and `<summary>` tags. These tags can be used in many ways, and are a great way to maximise page space. 

```
<details>
<summary>
<h2>Heading</h2>
</summary>
<p>
Content for accordion
</p>
</details>
```

I wasn't sure what the documentation would say about putting `<h2>` tags inside the `<summary>` element but, thankfully, **[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/summary)** states that permitted content includes *"Phrasing content or one element of Heading content."*

These collapsible content boxes allowed me to put the majority of my content on the homepage so the mobile user didn't have to keep scrolling back to a navbar to move around pages. Most of the information a recruiter would be looking for can be quickly expanded and collapsed without having to scroll at all.

<img align="right" style="margin: 20px" width="200" height="auto" src="./docs/component-images/galaxy-fold.png">

<a id="responsive"></a>
### Creating a responsive website:

[[back to top]](#top)

Both desktop and Samsung Galaxy Fold (in folded position) needed media queries. The latter was fairly straight forward; as the Samsung's screen is so small when folded, the main nav became
a bit of a mess. I simply changed the navbar to a column instead of
row and did a little re-positioning.

The desktop media query was a bigger task. My first approach was just throw a max-width on the column, and leave it in the centre, but initial feedback suggested that there was too much white space on the screen. After playing around with grid layout, I decided I would use it to turn the page into two main columns, with the expander boxes on
the left and the rest of the content on the right. Grid layout was a lot easier than I thought it would be to implement and I'm glad I did,
as the result was a much more immersive desktop experience.

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-home-light.png">

<a id="accessibility"></a>

### Creating an accessible and intuitive website:

[[back to top]](#top)

My biggest focus in this area was making sure to use semantic HTML, as well as making sure that all switches, filters and links were accessible via the tab, space and enter key. I also tested my portfolio's colours across different visual impairments. As I used the checkbox hack to build the theme-switch and blog category filters, I had to make sure to not just hide the checkbox, but rather shape it to the labels and make them transparent instead of setting them to `hidden`. This meant that although you can't see them, tabbing to the check-boxes creates an outline around the switch and filters, and allows them to be toggles or activated. I also added an aria-label to explain what the switch is for.

Mozilla Firefox's accessibility tools made it easy for me to see how my portfolio looked for people with different vision impairments, including Protanapia, Deuteranopia, Tritanopia and Achromatopsia; It also has a handy tool that displays your tab index order, which made it easy to check every page was tabbed correctly. I adjusted the contrast of my colours so that they would be suitable for people with low contrast, but also not too contrasted that it was difficult to read for people with no vision impairments. I also changed the areas which were highlighted when the theme was switched to dark mode, as bright yellow seems a lot brighter when the rest of the theme is dark.

Due to the simplicity of my site, there wasn't much I had to fix up to get a Lighthouse Accessibility score of 100%. All I had to do was add an aria-label to the resume download link and alt text to all of the images on the site.

<img style="margin: 20px" src="./docs/component-images/lighthouse.png">

<img style="margin: 20px" src="./docs/component-images/accessibility.png">

---

## <a id="sitemap"></a> Sitemap
[[back to top]](#top)

The sitemap for my portfolio is fairly straight forward; considering most of the content is contained on the homepage, the only other page required was a blog archive. A post navigator is included at the bottom of each blog post, in case the reader is enjoying my content and would like to keep reading; this makes for a smooth transition between blog posts, with no extra steps.

I also included a **Recent Posts** section on the homepage, which acts as another entry point into the blog post loop. The home page also has a link to my resume download and external links to my professional social media accounts.

<img style="margin: 20px" height="auto" src="./docs/site-map.png">

---

## <a id="screenshots"></a> Screenshots

<a id="mobile"></a>

[[back to top]](#top)

### Mobile Screenshots

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-home-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-home-dark.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-blog-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-blog-dark.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-post-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/mobile-post-dark.png">

<a id="desktop"></a>

### Desktop Screenshots

[[back to top]](#top)

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-home-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-home-dark.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-blog-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-blog-dark.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-blog-light-filtered.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-post-light.png">

<img style="margin: 20px" height="auto" src="./docs/screenshots/desktop-post-dark.png">

---
