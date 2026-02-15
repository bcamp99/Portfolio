---
layout: page
title: About <em>Me</em>
permalink: /about/
image: images/Headshot.jpg

---
My journey from operational leadership to design began with a simple realization: the best systems aren't just efficient—they're irresistible to the people who use them.

With a background in psychology (BA, USC) and years of experience leading operations in government contracting, I've seen how design can make or break engagement. My psychology training taught me how people think and decide; my operations work showed me how those insights hold up under pressure. Together, they fuel my belief that great design isn't just about aesthetics—it’s about creating experiences people genuinely want to return to.

> “No matter what anybody tells you, words and ideas can change the world.”
> <cite>Dead Poets Society</cite>

**My Design Philosophy**

I believe great design anticipates needs before users even realize them. It feels effortless, grounded, and magnetic — the kind of experience that keeps people coming back because it just makes sense.


**What I Bring**

- Psychology-informed insights into user motivation  
- Operational expertise in building systems that work under pressure  
- Strategic thinking that aligns design with organizational goals  
- A drive to craft experiences users love, not just use

My work blends design, psychology, and strategy to build experiences that feel good to use — not just good to look at. It’s about making things people actually want to come back to.

<script>
const url = "{{ '/docs/Bayley_E_Camp_2026_Tech_Resume.pdf' | relative_url }}";

const container = document.getElementById('pdf-container');

pdfjsLib.GlobalWorkerOptions.workerSrc = 'https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.8.162/pdf.worker.min.js';

pdfjsLib.getDocument(url).promise.then(pdf => {
  for (let pageNum = 1; pageNum <= pdf.numPages; pageNum++) {
    pdf.getPage(pageNum).then(page => {
      const viewport = page.getViewport({ scale: 1.2 }); // scale = zoom level
      const canvas = document.createElement('canvas');
      canvas.style.display = 'block';
      canvas.style.margin = '20px auto';
      const context = canvas.getContext('2d');
      canvas.height = viewport.height;
      canvas.width = viewport.width;
      container.appendChild(canvas);
      page.render({ canvasContext: context, viewport: viewport });
    });
  }
});
</script>

***