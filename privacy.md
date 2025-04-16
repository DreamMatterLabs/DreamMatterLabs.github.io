---
layout: default
title: "Privacy Policy"
permalink: /privacy/
---
<section style="background-color: #3D144E">
    <article class="col-8 col-md-5 post">
        <header class="post-header">
            <h1 class="post-title">Privacy Policy</h1>
            <p class="post-meta">March 24, 2025 ✧˚- Dream Matter Labs</p>
        </header>

        <div class="post-content" style="color: #f1e1f7">
	    <h2 class="post-heading">Overview</h2>

	    <p>This privacy policy applies to the website of Dream Matter Labs (“we” / “us” / "our") and carefully outlines our practices regarding your personal information. Do note that we may update this from time to time based on operational, regulatory, or legal reasons.</p>
	 
	    <h2 class="post-heading">Data Collection</h2>
      
	    <p>We strictly use analytics cookies that allow us to track website traffic and improve our content. Specifically, these are <a class="post-link" href="http://www.allaboutcookies.org" target="_blank">cookies</a> (i.e. small data files stored on your device) that collect information about your device and how you interact with our website.</p>

            <p>This may include your IP address, browser type, pages viewed, and the time spent on each page. This information helps us understand how visitors use our site and what content they find most interesting.</p>

	    <p>Moreover, we do this through Google Analytics, which collects information in a way that does not directly identify anyone and anonymizes IP addresses where possible. For more information on how Google collects and processes data, visit their <a class="post-link" href="https://www.google.com/intl/en/policies/privacy/">privacy policy</a>.</p>

            <button id="btn-consent" class="btn btn-rounded w-100 overflow-hidden text-nowrap text-truncate" style="margin-bottom: 15px" onclick="toggleConsent()">Click here to opt out</button>

	    <h2 class="post-heading">Contact Us</h2>

            <p>If you have any questions or complaints, please contact us <a class="post-link" href="mailto:{{ site.email }}">here</a>.</p>		 
        </div>
    </article>

    <script>
        function toggleConsent()
        {
            const consent = localStorage.getItem('ga-consent');

            if (consent != null)
            {
                if (consent === 'granted')
                {
                    localStorage.setItem('ga-consent', 'denied');
                    location.reload();
                }
                else
                {
                    localStorage.setItem('ga-consent', 'granted');
                    location.reload();
                }
            }          
        }

        (function checkConsent()
        {
            const consent = localStorage.getItem('ga-consent');

            if (consent != null)
            {
                if (consent === 'granted')
                {
                    document.getElementById('btn-consent').textContent = "Click here to opt out";
                }
                else
                {
                    document.getElementById('btn-consent').textContent = "Click here to opt in";
                }
            }
        })();
    </script>
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
    }
	
    .post-heading {
	color: white;
        font-size: 1.50rem;
        font-weight: bold;
        margin: 25px 0 25px 0;
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