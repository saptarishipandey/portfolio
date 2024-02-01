# Data Portfolio

### About me

Hi! I'm Saptarishi. I recently graduated from Simon Business School with an MS in Marketing Analytics. My dream is to get into data science. This website houses some of my projects in this field. I'm interested in machine learning, natural language processing, and computer vision.

:)

### Projects

<a href="https://github.com/saptarishipandey/Non-alcoholic-beer/tree/main" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">**Data driven perceptual mapping**</a>

* Created a perceptual map of 20 competing CPG Non-alcoholic beer products from internet ratings and reviews using principal component analysis and dimension reduction.
* Wrote a Python program that automated data gathering about 20 competing non alcoholic beer products from internet forums saving market research time significantly.
* _Tools used: Python, R, Reticulate Package, Beautiful Soup, Requests, Principal component analysis and dimension reduction_

<a href="https://github.com/saptarishipandey/Project-GMNL-Pricing-Choice-Models" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">**Is my price right? Price optimization and positioning of CPG products using Logistic Regression and Unsupervised Machine Learning**</a>

* Analyzed consumer preferences for a newly launched CPG product by leveraging multinomial logistic regression and  K-means clustering, utilizing data capturing choices of 359 consumers in different demographic groups over 3 years.
* Evaluated price elasticity to understand substitution patterns, unveiling insights into competitive product dynamics. Clustered consumers into 8 demographic segments and created price discrimination opportunities to discover 15% higher profits than static pricing.
* Recommended optimal pricing strategies, enhancing profit projections by 36%. Simulated a potential pricing war scenario with competing brand, iteratively adjusting prices to determine equilibrium points, which informed strategic decisions to launch the new product from the market.
* _Tools/skills used: Data analysis, R, statistical packages (gmnl), multinomial logistic regressions_

<a href="https://github.com/saptarishipandey/Home-Equity-Loan-Classification" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">**Home Equity Loan Classification**</a>

* Devised a machine learning approach for classifying home equity loan applicants as risky or not risky based on past delinquencies with 78% true positive rate and high interpretability using a logistic regression classifier on Python. <a href="https://github.com/saptarishipandey/Home-Equity-Loan-Classification/blob/main/HELOC%20classifier%20model.html" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">Full report</a>.

<div class="container container-custom" style="margin-top: 90px">
  {% for post in site.posts limit:3 %}
    {% if post.category == 'working papers' or post.category == 'publications' %}
      <div class="post">
        <a class="post__title" {% if post.pdf-url %}href="{{ post.pdf-url }}" target="_blank"{% endif %}>
          {{ post.title }}
        </a>
        <div class="post__subtitle">
          {{ post.co-authors }}
          {% if post.awards.size > 0 %}
            <ul>
              {% for award in post.awards %}
                <li>{{ award }}</li>
              {% endfor %}
            </ul>
          {% endif %}
        </div>
      </div>
    {% endif %}
  {% endfor %}
</div>

<div class="text-center" style="margin-top: 80px">
  <a class="btn btn-custom" href="/research.html">ALL RESEARCH ></a>
</div>
