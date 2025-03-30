---
layout: default
title: "Privacy Policy"
permalink: /privacy/
---
<article class="post">
    <header class="post-header">
        <h1 class="post-title">Privacy Policy</h1>
        <p class="post-meta">March 24, 2025 • Dream Matter Labs</p>
    </header>

    <div class="post-content">
	<h2 class="fs-4 fw-bold">Overview</h2>

	<p>At Dream Matter Labs, your privacy is important to us and we will always try to treat you and your personal information with care and respect. Consequently, this Privacy Policy outlines our privacy practices regarding your personal information. We may update this from time to time based on personal, operational, legal, or regulatory reasons.</p>

	<h2 class="fs-4 fw-bold">Data Collection</h2>

   	{% if site.analytics.google %}
        <p>When you visit the Dream Matter Labs website, we automatically receive information about your device from your browser, such as your IP address. As you browse this website, we also collect information about how you interact with it. We refer to this automatically-collected information as “Device Information”. We collect Device Information using cookies. “Cookies” are data files that are placed on your device. For more information about cookies and how to disable them, visit http://www.allaboutcookies.org. We do this using Google Analytics: <https://www.google.com/intl/en/policies/privacy/>. You can opt-out of Google Analytics here: <https://tools.google.com/dlpage/gaoptout>.</p>
        {% else %}
        <p>We do not collect any of your personal data nor make use of cookies.</p>
        {% endif %}

        <h2 class="fs-4 fw-bold">Contact Us</h2>

        <p>If you have questions or complaints, please contact us at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.</p>
    </div>
</article>

<style>
    .post {
        max-width: 800px; /* Keeps content width readable */
        margin: 150px auto; /* Centers content with spacing */
        font-size: 1.25rem;
    }

    .post-header {
        margin-bottom: 50px;
        text-align: center;
    }

    .post-title {
        font-size: 2.45rem;
        margin-bottom: 10px;
        font-weight: bold;
    }

    .post-meta {
        font-size: 1.25rem;
        color: #666; /* Subtle color for metadata */
        margin-bottom: 0;
    }

    .post-banner {
        width: 100%;
        aspect-ratio: 16 / 9;
        box-shadow: 0px 0px 15px 5px rgba(0, 0, 0, 0.25);
        margin-bottom: 50px;
    }

    .post-content {
        line-height: 1.6;
        margin-bottom: 40px;
    }
</style>