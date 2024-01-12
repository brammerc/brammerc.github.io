---
layout: page
title: Connect
---

# Connect

#### Contact us if you have questions or comments about the contents of this website, or if you are interested in collaborating on your data science project

<hr/>

## Email

<form id="contactform" method="POST">
  <div class="half left form-group">
    <input type="text" name="Name" class="form-control" style="margin-bottom:3px;" placeholder="Name">
    <input type="email" name="Email" class="form-control" style="margin-bottom:3px;" placeholder="Email address (I will NOT share)">
    <input type="text" name="Subject" class="form-control" placeholder="Subject">
    <input type="hidden" name="_subject" value="SPA contact form" />
    <input type="text" name="_gotcha" style="display:none" />
  </div>
  <div class="half right form-group">
    <input type="hidden" name="_next" value="http://localhost:4000/contact/thanks.html" />
    <textarea name="Message" class="form-control" rows="5" placeholder="Message"></textarea>
  </div>
  <div class="form-group">
    <input class="btn btn-primary" type="submit" value="Submit">
  </div>
</form>
<script>
    var contactform =  document.getElementById('contactform');
    contactform.setAttribute('action', '//formspree.io/' + 'sportperformanceanalytics' + '@' + 'gmail' + '.' + 'com');
</script>

<hr>

## Want to Collaborate?
If you would like to collaborate on a data project within the recreational and competitive swimming domains, we are available for contract and consultation on measurement, data processing, data analysis, data visualization, and/or data interpretation. Please email a brief proposal that includes the following:

- a description of the problem that the project aims to solve 
- your motivation for tackling this problem
- the role that you envision we will play (e.g., consultant, contractor)
- a description the potential data source(s)

## Services

#### We work with stakeholders in the recreational and competitive swimming domain that value the use of data-derived insights to facilitate the decisions they make

<hr/>

I am available for contract and consultation on measurement, data processing, data analysis, and/or data interpretation within the health, physical activity, and sports domains. 

I aim to help organizations use data to discover new information, develop explanatory models of the past, and predict future performance outcomes. 

Contact me to assist in projects that require any of the following: 
- Valid and reliable measurement of physiological, biomechanical, and motor control variables
- Scraping data from web sources 
- Data acquistion, cleaning, management
- Data processing and analysis using R and Python
  - Population parameter estimation and hypothesis testing (Chi-square, ANOVA, linear mixed effects models)
  - Exploratory data analysis (data displays, re-expression, evaluating distributions, standardization, robust regression)
  - Time series analysis (smoothing techniques, spectral analysis, autoregressive (AR) and moving average (MA) models)
  - Multivariate analysis (MANOVA, PCA, factor analysis)
- Creating dynamic & reproducible data displays and summaries (dashboards, web applications) of analytical results using Shiny, ggplot2, and Plotly

## Platforms

All of my work leverage cutting-edge tools for data science. The following tools are in my wheelhouse:
  
- AWS (S3, EMR, Sagemaker, Cloudformation, Lambda)
- Docker
- Python (scikit-learn, tensorflow, pandas, xgboost)