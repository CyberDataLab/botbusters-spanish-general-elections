# Botbusters - Analysis of the 2019 Spanish General Election

This is the official repository for the Botbusters analysis of the 2019 Spanish General Election. 

[![Preprint](https://webs.um.es/mattia.zago/images/BB10N-Badge-ArXiV.svg)](https://arxiv.org/abs/2004.00931)
[![Dataset](https://webs.um.es/mattia.zago/images/BB10N-Badge-Data.svg)](http://dx.doi.org/10.21227/30ca-eg80)
[![Code](https://webs.um.es/mattia.zago/images/BB10N-Badge-Code.svg)](https://doi.org/10.5281/zenodo.3733195)

To cite this code repository, please use the following BibTeX. 
```
@misc{Botbusters10N, 
  title     = {Botbusters - Analysis of the 2019 Spanish General Election},
  author    = {Pastor-Galindo, J. and Zago, M. and Nespoli, P. and {Lopez~Bernal}, S. and {Huertas~Celdrán}, A. and {Gil~Pérez}, M. and Ruipérez-Valiente, J. A. and {Martínez~Pérez}, G. and {Gómez~Mármol}, F.}, 
  year      = {2020}, 
  month     = {Mar}, 
  version   = {DOI},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.3733195},
  url       = {https://github.com/CyberDataLab/botbusters-spanish-general-elections}
} 
```

The main article with the analysis of the data has been submitted for peer review. A preprint copy is available on arXiv [2]. 

The associated dataset has been published on IEEE Dataport [3]. 

## Authors
- Javier Pastor-Galindo (javierpg [at] um [dot] es) <sup>M</sup>
- Mattia Zago (mattia [dot] zago [at] um [dot] es) <sup>M</sup>
- Pantaleone Nespoli (pantaleone [dot] nespoli [at] um [dot] es) <sup>M</sup>
- Sergio López Bernal (slopez [at] um [dot] es) <sup>M</sup>
- Alberto Huertas Celdrán (ahuertas [at] tssg [dot] org) <sup>W</sup>
- Manuel Gil Pérez (mgilperez [at] um [dot] es) <sup>M</sup>
- José A. Ruipérez-Valiente (jruiperez [at] um [dot] es) <sup>M</sup>
- Gregorio Martínez Pérez (gregorio [at] um [dot] es) <sup>M</sup>
- Félix Gómez Mármol (felixgm [at] um [dot] es) <sup>M</sup>

## Affiliations
 <sup>M</sup> Authors are with the Department of Information and Communications Engineering, University of Murcia, Spain
 
 <sup>W</sup> Authors are with the Telecommunication Software & Systems Group, Waterford Institute of Technology, Ireland

## Abstract
>While social media has been proved as an exceptionally useful tool to interact with other people and massively and quickly spread helpful information, its great potential has been ill-intentionally leveraged as well to distort political elections and manipulate constituents. In the paper at hand, we analyzed the presence and behavior of political social bots on Twitter in the context of the November 2019 Spanish general election. Throughout our study, we classified involved users as Social bots or humans, and examined their interactions from a quantitative (i.e., amount of traffic generated and existing relations) and qualitative (i.e., user's political affinity and sentiment towards the most important parties) perspectives. Results demonstrated that a non-negligible amount of those bots actively participated in the election, supporting each of the five principal political parties.

## Usage
There are five notebooks to perform the analysis of the data [3]. To be precise:
- [Phase 1](notebooks/Phase1.ipynb) takes care of importing, checking, completing, and formatting the raw data retrieved from the Social Feed Manager [4].
- [Phase 2](notebooks/Phase2.ipynb) preprocess the data in order to calculate the required features. It also anonymizes the data for the analysis.
- [Phase 3](notebooks/Phase3.ipynb) extracts the statistical information regarding the social bots' activities.
- [Phase 4](notebooks/Phase4.ipynb) processes the data for the social bots' classification, which is performed with Orange3 [5]. The friendship graph is drawn with Gephi [6].
- [Phase 5](notebooks/Phase5.ipynb) performs the analysis of the results provided by the social bots' classification process.

## Bibliography
1. Zago M., Nespoli P., Papamartzivanos D., Gil Pérez M., Gómez Mármol F., Kambourakis G. and Martínez Pérez G., 2019. **Screening Out Social Bots Interference: Are There Any Silver Bullets?**. _IEEE Communications Magazine_, 57(8), pp.98-104. DOI: [10.1109/MCOM.2019.1800520](https://dx.doi.org/10.1109/MCOM.2019.1800520)
2. Pastor-Galindo J., Zago M., Nespoli P., López Bernal S., Huertas Celdrán A., Gil Pérez M., Ruipérez-Valiente J. A., Martínez Pérez G., Gómez Mármol F., 2020. **Spotting political social bots in Twitter: A use case of the 2019 Spanish general election**. _arXiv preprint [arXiv:2004.00931](https://arxiv.org/abs/2004.00931)_
3. Pastor-Galindo J., Zago M., Nespoli P., López Bernal S., Huertas Celdrán A., Gil Pérez M., Ruipérez-Valiente J. A., Martínez Pérez G., Gómez Mármol F., 2020. **Spotting political social bots in Twitter: a dataset for the 2019 Spanish general election**. _IEEE Dataport_. DOI: [10.21227/30ca-eg80](https://dx.doi.org/10.21227/30ca-eg80)
4. George Washington University Libraries, 2016. **Social Feed Manager**. _Zenodo_. DOI: [10.5281/zenodo.597278](https://dx.doi.org/10.5281/zenodo.597278)
5. Demsar J., Curk T., Erjavec A., Gorup C., Hocevar T., Milutinovic M., Mozina M., Polajnar M., Toplak M., Staric A., Stajdohar M,. Umek L., Zagar L., Zbontar J., Zitnik M., Zupan B., 2013. **Orange: Data Mining Toolbox in Python**. _Journal of Machine Learning Research_. vol. 14, Aug 2013, p. 2349−2353.
6. Bastian, M., Heymann, S., Jacomy, M., 2009. **Gephi: An Open Source Software for Exploring and Manipulating Networks**. _Third International AAAI Conference on Web and Social Media_.
