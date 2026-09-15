
Documentation · MD
# Project Documentation. My Personal Portfolio Website
 
Sarah Kruschinski · Web Programming SS26 · Leuphana University
Live site: https://sasokru.github.io
 

 
## 1. in General
 
My website project is a multi-page personal portfolio website, built with 
HTML and CSS and deployed on GitHub Pages. It consists of four pages:
 
. **About** (`index.html`) — introduction, short bio, CV overview
. **drip.py** (`drip.html`) — deep-dive on my Arduino/Kalman-filter final project from TechBasics II
. **Writing** (`essay.html`) — web version of my Critical AI Studies essay on medical AI
. **Digital Health** (`news.html`) — a curated, hand-kept reading list of digital health sources

 
## 2. Design process
 
I started with just one page. That was the plan for the intermediate presentation as I needed something to show what the site was even about, what I wanted content-wise. It was also just easier to build at first.
 Pretty quickly I noticed it was way too much content for one page and that a nav bar at the top would work so much better. I was actually torn for a while; should the whole site be about drip.py, or about me? I ended up deciding it should be about me, and drip.py gets its own page you can click into from there. I like having that overview of myself and of digital health, because that's genuinely what I care about professionally.
 This probably isn't the website I'd actually use long-term, but it's a good foundation the HTML structure,which I would use to build up more for whatever comes after. :)
 From the start I wanted the design minimalist and I looked around online, found a few Pilates studio websites I liked, and used that as my reference, I wanted it to be clean, modern and kind of black-and-white. I also did Figma wireframes, which was part of the course exercise. Handling Figma was honestly hard for me at first. But I used it to sketch out that same minimal approach, and fitting all my content into one wireframe was really difficult, which is part of why I moved to multiple pages in the end.
 Honestly, the more interesting part for me was the technical side and hoping it would work to link pages together and getting images and files and links embedded properly.It was also quite hard to make the nav bar actually work across every page. The minimal design was a deliberate choice the whole way through as I wanted my work in the foreground.
 
 
## 3. Technical implementation
 
**Layout**
- Every page shares a single `style.css` for consistent structure across the site
- Primary layout technique: **CSS Flexbox**  used for the nav bar, hero sections,
  the project index rows, two-column feature sections, and the footer
- **Position** is used selectively: e.g. absolute-positioned captions/labels on
  images, and structural anchoring in a few components
- **Responsive design**: a `@media` query adjusts layout below 820px so columns
  stack on mobile
- Typography: **Instrument Sans** for headings, **Inter** for body text , both
  clean sans-serif fonts , loaded via Google Fonts
**Structure**
- Each page uses semantic sectioning (`<header>`, `<nav>`, `<main>`, `<section>`,
  `<footer>`)
- Shared navigation appears on every page, with a `.current` class marking the
  active page
- Images live in a shared `/images` folder; downloadable documents (essay, project
  report) sit alongside the HTML files in the repository root
 
## 4. Libraries, tools & references
 
 I used Google Fonts for the typography, Figma for the wireframes before I started coding, VS Code as my editor, and Git with GitHub Pages for hosting, just as we were taught in the seminar. For reference when I got stuck, I mostly used MDN Web Docs.
 
 
## 5. AI use disclosure
 I used Claude (Anthropic) throughout this project, for a part of the technical implementation. Specifically:
 
- Claude wrote the initial HTML and CSS for the site's intermediate presentation version
- I used it to troubleshoot GitHub Pages deployment issues
- I used it for writing the HTML code of the nav bar
-I used it to help implement a style inspo I found online by identifying the font and the CSS in general
- I used it for help when I did not know a certain skill in HTML and CSS (like the nav bar and adding a link to a downloadable document) and let it explain it to me, 
then typing it myself and putting the code together

The code I wrote needed real back-and-forth from Claude to get right, sometimes leading to rebuilding the font and design direction. To me it was always important to understand the
feedback and the output it gave me, so that i could apply it. Which also led to certain things, like a generator for digital health news not being included, because it really exceeded
my level of understanding...
 
## 6. Reflection
 
**What was the hardest part?**
 
Definitely creating a page that felt clean and übersichtlich and figuring out where each piece of content should go was genuinely interesting, especially with several different topics (myself, drip.py, the essay, digital health) that all needed their own space without the site feeling cluttered.
 Finding a CSS style that actually fit me was hard too. We ended up with Instrument Sans for headings and Inter for body text. The hard part wasn't picking fonts, but staying disciplined not overdoing it to stick to the minimalist tone I'd set for myself from the start. 
 Structuring my GitHub repository logically was also harder than I expected, especially keeping the images, the essay files, and all the other uploaded documents organized in a way that actually made sense.
I'm genuinely proud of the digital health reading list page. It's hand-picked, which isn't as impressive as something automated or dynamically generated but I wasn't able to build an actual generator for it as stated above, so I put real thought into which sources I actually like and picked those.
The drip.py page was probably the hardest part overall: the images, the spec tables, and getting everything from the project properly represented, it took the most work to get right.
 
**What would I do differently?**
 
I would have started deciding on what I actually wanted the page to be about earlier. I changed direction after the intermediate presentation, going from a drip.py-centered idea to a page about myself. Looking back, that detour was actually useful as it helped me realize what I didn't want.
Even though I like the clean, minimal result, I still feel like the page isn't quite as calm and cleanly designed as I originally wanted. I tried my best to not overload it and to give things proper spacing, but if I did it again I might reconsider going quite so minimalistic.
 The other thing I'd do differently is my workflow with files — I kept having to sit down and fix small things again and again, and a few times I put files in the wrong folder and had to delete and re-upload them. Next time I'd try to add all the files and images together, in one clean pass, rather than piecing it together over several sessions.
 
**What's still left before September 15?**
 
At this point I've actually finished what I set out to do structurally. All four pages exist and are linked correctly. My last steps were adding a few missing images and files that I'd forgotten to upload to GitHub, which caused some links and pictures not to work. Writing this documentation was also one of the last steps as I actually had to look back through my commit history to remember what I'd done and when, which made me realize the commits themselves are kind of a documentation in their own right.
