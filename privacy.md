---
layout: default
title: "Privacy Policy"
permalink: /privacy/
---
<section style="background-color: #6B2489">
    <article class="col-8 col-md-5 post">
        <header class="post-header">
            <h1 class="post-title">Privacy Policy</h1>
            <p class="post-meta">March 24, 2025 ✧˚- Dream Matter Labs</p>
        </header>

        <div class="post-content">
	    <h2 class="fs-4 fw-bold">Overview</h2>

	    <p>At Dream Matter Labs, your privacy is important to us and we will always try to treat you and your personal information with care and respect. Consequently, this Privacy Policy outlines our privacy practices regarding your personal information.</p>

            <p>We may update this from time to time based on operational, regulatory, or legal reasons.</p>

            <p>If you have questions or complaints, please contact us <a class="post-link" href="mailto:{{ site.email }}">here</a>.</p>	
	    		 
	    <h2 class="fs-4 fw-bold">Data Collection</h2>
      
   	    {% if site.analytics.google %}
            <p>When you visit the Dream Matter Labs website, we automatically receive information about your device from your browser, such as your IP address. As you browse this website, we also collect information about how you interact with it. We refer to this automatically-collected information as “Device Information”. We collect Device Information using cookies. “Cookies” are data files that are placed on your device. For more information about cookies and how to disable them, visit http://www.allaboutcookies.org. We do this using Google Analytics: <https://www.google.com/intl/en/policies/privacy/>. You can opt-out of Google Analytics here: <https://tools.google.com/dlpage/gaoptout>.</p>
            {% else %}
            <p>We do not collect any of your personal data nor make use of cookies.</p>
            {% endif %}
        </div>
    </article>
</section>

<style>
    .post {
        margin: 0 auto;
	padding: 150px 0 150px 0;
	color: white;
    }

    .post-header {
        margin-bottom: 50px;
        text-align: center;
    }

    .post-title {
        font-size: 2.5rem;
        font-weight: bold;
        margin-bottom: 15px;
    }

    .post-meta {
        font-size: 1.25rem;
        color: #B7FDFE;
        margin-bottom: 0;
    }

    .post-content {
        font-size: 1.25rem;
        line-height: 1.6;
        margin-bottom: 50px;
    }

    .post-link {
        color: #B7FDFE;
        text-decoration: none;
	font-weight: bold;
    }

    .post-link:hover {
        color: #C5FDFE;
        text-decoration: underline;
    }
</style>