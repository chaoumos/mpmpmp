---
import Layout from '../../layouts/BlogPost.astro';

export const frontmatter = {
  title: 'Welcome to the mpmpmpmp Blog!',
  description: 'A brief introduction to our AI and automation blog.',
  pubDate: '2024-07-03',
  layout: '../../layouts/BlogPost.astro'
};

const { title, description, pubDate } = frontmatter;
---

<Layout title={title} description={description}>
  <article class="prose lg:prose-xl">
    <h1>{title}</h1>
    <time datetime={pubDate}>{new Date(pubDate).toLocaleDateString()}</time>
    <p>
      Welcome to the mpmpmpmp blog! We are excited to share our insights and expertise on the latest trends in AI and automation.
    </p>
    <p>
      In this blog, you'll find articles, tutorials, and case studies covering a wide range of topics, including:
    </p>
    <ul>
      <li>Machine Learning</li>
      <li>Robotic Process Automation (RPA)</li>
      <li>AI-powered Business Solutions</li>
      <li>The Future of Work</li>
    </ul>
    <p>
      Stay tuned for regular updates and be sure to subscribe to our newsletter to never miss an article!
    </p>
  </article>
</Layout>