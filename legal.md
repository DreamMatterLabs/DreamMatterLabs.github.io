---
layout: default
title: Privacy Policy
---
<section class="page-section" style="background: linear-gradient(to bottom, #5B0557, #3A4175, #423B7A)" id="{{ site.data.sitetext[site.locale].team.section | default: "team" }}">
    <div class="container d-flex flex-column" style="padding-top: 50px; padding-bottom: 50px; row-gap: 150px">
        <!--Tagline-->
        <div class="section-header text-center">
            <h1 class="m-0 fs-4 text-uppercase text-muted2">Privacy Policy</h1>
        </div>

        <!--Information-->
        <div class="row d-flex justify-content-center">
	    <p>This Privacy Policy describes how your personal information is collected, used, and shared when you visit {{ site.title }} (the “Site”).</p>

	    <h2>PERSONAL INFORMATION WE COLLECT</h2>

	    <p>This Privacy Policy describes how your personal information is collected, used, and shared when you visit {{ site.title }} (the “Site”).</p>

	    {% if site.analytics.google %}
	    <h2>Automatically Collected (Google Analytics)</h2>

	    <p>When you visit the Site, we automatically receive information about your device from your browser, such as your IP address. As you browse the Site, we also collect information about how you interact with the Site. We refer to this automatically-collected information as “Device Information”. We collect Device Information using cookies. “Cookies” are data files that are placed on your device. For more information about cookies and how to disable them, visit http://www.allaboutcookies.org. We do this using Google Analytics: <https://www.google.com/intl/en/policies/privacy/>. You can opt-out of Google Analytics here: <https://tools.google.com/dlpage/gaoptout>.</p>
	    {% else %}
	    <p>We do not collect any data about you or use any cookies.</p>
	    {% endif %}

	    <h2>CHANGES</h2>

	    <p>We may update this privacy policy from time to time for personal, operational, legal, or regulatory reasons.</p>

	    <h2>CONTACT US</h2>

	    <p>For more information about our privacy practices or if you have questions, please contact us by email at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.</p>
        </div>
    </div>
</section>