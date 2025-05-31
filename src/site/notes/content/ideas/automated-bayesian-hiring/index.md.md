---
{"dg-publish":true,"permalink":"/content/ideas/automated-bayesian-hiring/index-md/"}
---

# Automated Bayesian Hiring Predictor

_Status_: In Progress  
_Last Updated_: May 31, 2025  
_Tags_: #in-progress #bayesian #ml #careers  

---

## Overview  
Can we build a system that estimates your probability of getting hired into a specific role based on previous applicant data — especially their outcomes and portfolios — and compare that with your own?

---

## Motivation  
Hiring feels noisy and opaque. But over time, patterns emerge.  
If we had access to historical data — who applied, what their CVs looked like, who got offers — could we model this probabilistically?  
Even without full data, can we prototype the mechanics of such a system?

---

## First Thoughts  
![](/img/user/content/ideas/automated-bayesian-hiring/bays.png)
- Bayes' theorem is natural for this: updating belief in acceptance probability given similarity to successful applicants.  
- Inputs:  
  - Your CV vector  
  - Past applicants’ CVs  
  - Outcomes (offer/reject)  
- Could use vector embeddings (e.g. from resumes) and similarity metrics  
- Open questions:  
  - How do we simulate historical data?
  - How do we define “CV similarity” in a useful way?

---

## 📈 Version History

### v0.1 — May 31, 2025  
Initial outline and hypothesis.

---

## Work Log

### [May 31, 2025]  
Wrote project outline. Considering embedding models to represent CVs.  
Thinking about how to define a “prior” over acceptance rates.

---

## Technical Notes  
- Consider using cosine similarity over document embeddings  
- Logistic regression or simple Bayes classifier as baseline  
- Could try a probabilistic programming framework (e.g., Pyro)

---

## Next Steps  
- Write simulation code for past applicants and outcomes  
- Explore embedding approaches for resume text  
- Sketch a naive Bayes-style formulation
