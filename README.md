# Multimodal disease progression: five small experiments

An interactive demo prepared for the PhD in Machine Learning in Medicine (University of Bern). Each tab takes one focus area from the project description and shows it on a simulated cohort of 600 patients with imaging, wearable and tabular measurements.

**Live demo:** https://sanafirdouse2323-glitch.github.io/disease-progression-experiments/

| Tab | Focus area | What it shows |
|---|---|---|
| Multimodal fusion | Multimodal representation learning | Reliability-weighted latent stage estimate versus each modality alone |
| Sparse longitudinal | Progression from cross-sectional and sparse longitudinal data | Aligning patients with few visits onto one disease timeline |
| Causal effect | Disentangling progression from treatment effects | Confounded treatment assignment: naive versus stratified estimate versus the true effect |
| Missing data | Missing modalities and irregular sampling | Zero-fill versus observed-only weighting |
| Fairness | Bias across subgroups | A less reliable sensor for one subgroup, with and without group-aware weights |

## Limits

All data are synthetic, generated from a latent disease stage per patient. The methods are deliberately simple statistical stand-ins (precision-weighted fusion, pooled slopes, stratification) that expose each problem. They are not clinical results and not the learned models a real study would use.

## Run locally

Open `index.html` in a browser. There is no build step and no dependencies apart from a web font.

## Possible next steps

Replace the stand-ins with learned models (a multimodal encoder, a mixed-effects or neural progression model, a causal estimator such as doubly robust learning) and evaluate on public medical datasets.
