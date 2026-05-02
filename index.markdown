---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---
<style>
  .sicss-announcement {
    align-items: center;
    background: #f9fafb;
    border: 1px solid #e5e7eb;
    border-left: 5px solid #4b2e83;
    border-radius: 6px;
    display: flex;
    gap: 18px;
    margin: 0 0 22px;
    padding: 16px 48px 16px 18px;
    position: relative;
  }

  .sicss-announcement[hidden] {
    display: none;
  }

  .sicss-announcement__image {
    border-radius: 4px;
    flex: 0 0 112px;
    height: 112px;
    object-fit: cover;
    width: 112px;
  }

  .sicss-announcement__headline {
    color: #111827;
    font-size: 1.2rem;
    font-weight: 600;
    line-height: 1.25;
    margin: 0 0 4px;
  }

  .sicss-announcement__date {
    color: #4b2e83;
    font-size: 0.95rem;
    font-weight: 600;
    line-height: 1.35;
    margin: 0 0 8px;
  }

  .sicss-announcement__body {
    color: #374151;
    font-size: 1rem;
    line-height: 1.5;
    margin: 0;
  }

  .sicss-announcement__dismiss {
    background: transparent;
    border: 0;
    border-radius: 4px;
    color: #6b7280;
    cursor: pointer;
    font-size: 1.6rem;
    height: 32px;
    line-height: 1;
    padding: 0;
    position: absolute;
    right: 8px;
    top: 8px;
    width: 32px;
  }

  .sicss-announcement__dismiss:hover,
  .sicss-announcement__dismiss:focus {
    background: #eef2f7;
    color: #111827;
  }

  @media screen and (max-width: 560px) {
    .sicss-announcement {
      align-items: flex-start;
      gap: 12px;
      padding: 14px 42px 14px 14px;
    }

    .sicss-announcement__image {
      flex-basis: 78px;
      height: 78px;
      width: 78px;
    }

    .sicss-announcement__headline {
      font-size: 1.05rem;
    }

    .sicss-announcement__body {
      font-size: 0.95rem;
    }
  }
</style>

<aside id="sicss-announcement" class="sicss-announcement" role="region" aria-labelledby="sicss-announcement-title">
  <img class="sicss-announcement__image" src="assets/sicss-uw-2026.png" alt="Computational Social Science Summer Institute badge" />
  <div class="sicss-announcement__content">
    <p id="sicss-announcement-title" class="sicss-announcement__headline">Summer Institute in Computational Social Science</p>
    <p class="sicss-announcement__date">July 6 to July 17, 2026</p>
    <p class="sicss-announcement__body">We're soliciting applications from graduate students, postdoctoral researchers, junior faculty, and data science practitioners. The program will have a special emphasis on AI-centered computational social science. More information &amp; application is here: <a href="https://sicss.io/2026/uw/">https://sicss.io/2026/uw/</a>.</p>
  </div>
  <button id="sicss-announcement-dismiss" class="sicss-announcement__dismiss" type="button" aria-label="Dismiss summer institute announcement">&times;</button>
</aside>

<script>
  (function() {
    var banner = document.getElementById('sicss-announcement');
    var dismiss = document.getElementById('sicss-announcement-dismiss');
    var storageKey = 'sicss-uw-2026-announcement-dismissed';

    if (!banner || !dismiss) {
      return;
    }

    try {
      if (window.localStorage.getItem(storageKey) === 'true') {
        banner.hidden = true;
        return;
      }
    } catch (error) {}

    dismiss.addEventListener('click', function() {
      banner.hidden = true;

      try {
        window.localStorage.setItem(storageKey, 'true');
      } catch (error) {}
    });
  })();
</script>

<figure>
  <img src="assets/tylerpic.jpg" style="padding: 10px; float: left; width:364.8px;height:273.6px;"/>
 </figure>
 My research covers a variety of topics in statistics and data science, typically motivated by scientific questions in global health, economics, demography, and sociology. Recent projects include estimating features of social networks (e.g. the degree of clustering or how central an individual is) using data from standard surveys, inferring a likely cause of death (when deaths happen outside of
hospitals) using reports from surviving caretakers, and quantifying & communicating uncertainty
in predictive models for global health policymakers. More information about OpenVA, our suite of open tools to manage and analyze verbal autopsy surveys, is available [here](http://openva.net/).
<br>

I'm the former Editor of the [Journal of Computational and Graphical Statistics](https://www.tandfonline.com/action/journalInformation?show=editorialBoard&journalCode=ucgs20) and a 2019 recipient of the [NIH Director's New Innovator Award](https://commonfund.nih.gov/newinnovator).  I was elected as a [Fellow](https://stat.uw.edu/news-resources/articles/adrian-dobra-and-tyler-mccormick-elected-2023-asa-fellows) of the [American Statistical Association](https://www.amstat.org/your-career/awards/asa-fellows) in 2023.
<br>

An description of some of our work recently appeared in the [Wall Street Journal](https://www.wsj.com/us-news/you-probably-know-611-people-heres-how-we-know-88dd27d9?mod=wsjhp_columnists_pos2) and it was used for a [visual story](https://www.washingtonpost.com/world/interactive/2024/gaza-numbers-killed-displaced-scale/?itid=ap_alyssafowers) in the Washington Post.
<br>

A link to my slides from the ASA Webinar on the role of statistics in AI is [here](https://docs.google.com/presentation/d/1uL2pO80lk1T5ahLi3vDFo5NDAMZ_wdnDIYGFk6xZ-Bg/edit?usp=sharing).
<br>

A new paper on the epidemiology of AI is [here](https://arxiv.org/abs/2604.14086).
<br>

A link to our ENAR short course is [here](https://thmccormick.github.io/ipd-short-course/).
<br>

### Technical reports and working papers
+ Measurement and modeling of social networks and peer influence
  + [Non-robustness of diffusion estimates on networks with measurement error](https://arxiv.org/abs/2403.05704) (Revise & Resubmit, *Econometrica.*)
  + [Randomized recruitment driven sampling](https://arxiv.org/abs/2603.00365)
  + [Scalable Spatial Stream Network (S3N) Models](https://arxiv.org/abs/2512.12398)
  + [Model-based inference and experimental design for interference using partial network data](https://arxiv.org/abs/2406.11940) ([R package](https://github.com/SteveJWR/SBMNetReg), [code](https://github.com/SteveJWR/ardexp))
  + [Asymptotically normal estimation of local latent network curvature](https://arxiv.org/abs/2211.11673) ([R package](https://github.com/SteveJWR/lolaR), [code](https://github.com/SteveJWR/netcurve))
  + [General covariance-based conditions for Central Limit Theorems with dependent triangular arrays](https://arxiv.org/abs/2308.12506)
  + [Estimating spillovers using imprecisely measured networks](https://arxiv.org/abs/1904.00136) [(code)](https://github.com/thmccormick/spillovers-mismeasured-graphs)
  + [Examining Racial Segregation in Associative Networks on Twitter](https://arxiv.org/abs/1705.04401)
+ Decision-making under uncertainty
  + [Robustly estimating heterogeneity in factorial data using Rashomon Partitions](https://arxiv.org/abs/2404.02141) ([Python package & code](https://github.com/AparaV/rashomon-partition-sets))
  + [Spatially robust inference with predicted and missing at random labels](https://arxiv.org/abs/2603.11368)
  + [REALITrees: Rashomon Ensemble Active Learning for Interpretable Trees](https://arxiv.org/abs/2603.22750)
  + [Adaptive active learning for regression via reinforcement learning](https://arxiv.org/abs/2603.10435)
  + [How to measure obesity in public health research? Problems with using BMI for population inference](https://www.medrxiv.org/content/10.1101/2025.04.01.25325037v1)
  + [When you come to a fork in the road, take it: the Rashomon effect for social scientists](https://osf.io/preprints/socarxiv/8zybt_v2)
  + [Some models are useful, but for how long?: A decision theoretic approach to choosing when to refit large-scale prediction models](https://arxiv.org/abs/2405.13926)
  + [Do we really even need data?](https://arxiv.org/abs/2512.05456)
  + [A unified framework for inference with general missingness patterns and machine learning imputation](https://arxiv.org/abs/2508.15162)
  + [A moment-based generalization to Post-Prediction Inference](https://arxiv.org/abs/2507.09119)
+ Global health methodology and data collection strategies
  + [LAVA: Language Model Assisted Verbal Autopsy for Cause-of-Death Determination](https://arxiv.org/abs/2509.09602)
  + [Feasible contact tracing](https://arxiv.org/abs/2312.05718)
  + [Smart containment with active learning: A proposal for a data-responsive and graded approach to COVID-19](https://www.hks.harvard.edu/centers/cid/publications/smart-containment-with-active-learning) [(more details)](https://www.cerp.org.pk/pages/covid-19-smart-containment-policy-response)
  + [Quantifying the contributions of training data and algorithm logic to the performance of automated cause-assignment algorithms for verbal autopsy](https://arxiv.org/abs/1803.07141)
  + [Bayesian age category reconciliation for age- and cause-specific under-five mortality estimates](https://arxiv.org/abs/2302.11058)
  + [Verbal autopsy in civil registration and vital statistics: The Symptom-Cause Information Archive](https://arxiv.org/abs/1910.00405)
  
  Please see [arXiv](https://arxiv.org/search/?searchtype=author&query=McCormick%2C+T) for the most up to date list of working papers.



### Affiliations
+ [University of Washington](http://www.uw.edu)
  + Professor, [Department of Statistics](http://www.stat.washington.edu/) and [Department of Sociology](https://soc.washington.edu/).
  + Core faculty member, [Center for Statistics and the Social Sciences](http://csss.washington.edu/). 
  + Senior Data Science Fellow, [eScience Institute](http://escience.washington.edu/).
  + Research affiliate, [Center for Studies in Demography and Ecology](https://csde.washington.edu/).
  + Faculty partner, [Responsible AI Systems & Experiences (RAISE)](https://www.raise.ischool.uw.edu/).
