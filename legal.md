---
layout: default
title: Privacy Policy
---
<article class="post">
    <header class="post-header">
        <h1 class="post-title">Privacy Policy</h1>
        <p class="post-meta">March 24, 2025 • Dream Matter Labs</p>
    </header>

    <div class="post-content">
	<p>This Privacy Policy describes how your personal information is collected, used, and shared when you visit {{ site.title }} (the “Site”).</p>

	<h2 class="fs-4 fw-bold">PERSONAL INFORMATION WE COLLECT</h2>

   	{% if site.analytics.google %}
        <p>When you visit the Site, we automatically receive information about your device from your browser, such as your IP address. As you browse the Site, we also collect information about how you interact with the Site. We refer to this automatically-collected information as “Device Information”. We collect Device Information using cookies. “Cookies” are data files that are placed on your device. For more information about cookies and how to disable them, visit http://www.allaboutcookies.org. We do this using Google Analytics: <https://www.google.com/intl/en/policies/privacy/>. You can opt-out of Google Analytics here: <https://tools.google.com/dlpage/gaoptout>.</p>
        {% else %}
        <p>We do not collect any data about you or use any cookies.</p>
        {% endif %}

        <h2 class="fs-4 fw-bold">CHANGES</h2>

        <p>We may update this privacy policy from time to time for personal, operational, legal, or regulatory reasons.</p>

        <h2 class="fs-4 fw-bold">CONTACT US</h2>

        <p>For more information about our privacy practices or if you have questions, please contact us by email at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.</p>
    </div>
</article>

<style>
    .post {
        max-width: 800px; /* Keeps content width readable */
        margin: 40px auto; /* Centers content with spacing */
        padding: 20px;
    }

    .post-header {
        margin-bottom: 20px;
        text-align: center;
    }

    .post-title {
        font-size: 2rem;
        margin-bottom: 10px;
    }

    .post-meta {
        font-size: 1rem;
        color: #666; /* Subtle color for metadata */
        margin-bottom: 20px;
    }

    .post-content {
        line-height: 1.6;
        margin-bottom: 40px;
    }
</style>