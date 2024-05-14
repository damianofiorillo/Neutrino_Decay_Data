# Neutrino_Decay_Data

Plotting scripts to generate and plot the present and projected joint two-dimensional bounds on neutrino lifetimes, from Figs. 5 and 6 of the paper *Neutrino decay in the cosmic high-energy diffuse and point-source fluxes* [arXiv:XXXX.XXXXX](http://arxiv.org/abs/XXXX.XXXXX).  

Also contains the pre-computed digitized contours for reusing them elsewhere.

## Contents
```
   README.md           				    The file that you are reading
   ImportingDigitizedContours.ipnyb  Jupyter notebook to import and plot pre-computed contours of neutrino lifetimes
   PlottingScript.ipnyb     		    Jupyter notebook to extract contours of neutrino lifetimes and make Figs. 5, 6 of the paper
   digitized_contours/               Contains the 95% C.L. pre-computed contours of $\tau_3/m_3$ vs.~$\tau_2/m_2$
      .../diffuse_contours/          Bounds extracted from the diffuse neutrino flux
      .../ngc1068_contours/          Bounds extracted from the neutrino flux from NGC1068
   likelihood_data/                  Contains the pre-compute likelihood from which to derive lifetime contours
      .../diffuse_contours/          Likelihood for the diffuse neutrino flux
      .../ngc1068_contours/          Likelihood for the neutrino flux from NGC1068
```

## How to use the code

### To import the pre-computed neutrino lifetime contours

The 95% C.L. pre-computed contours of disfavored $\tau_3/m_3$ vs.~$\tau_2/m_2$ shown in Figs. 5 and 6 of XXXX.XXXXX are stored in the folder `digitized_contours/`. Open the notebook `ImportingDigitizedContours.ipynb` to find how to import and plot them. This notebook simply __plots__ the pre-computed contours; to __generate__ them, see below.

### To generate new neutrino lifetime contours

The notebook `PlottingScript.ipnyb` contains code to generate the contours of disfavored $\tau_3/m_3$ vs.~$\tau_2/m_2$ using the pre-computed likelihood data stored in the folder `likelihood_data/`.  By default, the code generates the contours at 95% C.L., but the user can change this.

This notebook also contains code to generate Figs. 5 and 6 of XXXX.XXXX.

## Citing

If you use these results in your work, we ask you that you please cite the following paper: Víctor B. Valera, Damiano F. G. Fiorillo, Ivan Esteban and Mauricio Bustamante, *Neutrino decay in the cosmic high-energy diffuse and point-source fluxes* ([arXiv:XXXX.XXXXX](http://arxiv.org/abs/XXXX.XXXXX)).

If you are citing our work in a document that will be uploaded to the arXiv, please consider using the LaTeX or BibTeX entries provided by INSPIRE ([link here](http://inspirehep.net/record/XXXXX/export/hx)):
```
@article{XXXXX,
      author         = "XXXX",
      title          = "{XXXX}",
      year           = "22024",
      eprint         = "XXXX.XXXX",
      archivePrefix  = "arXiv",
      primaryClass   = "hep-ph",
      SLACcitation   = "%%CITATION = ARXIV:XXXX.XXXXX;%%"
}
```