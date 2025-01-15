# Tracking the Takes and Trajectories of News Narratives from Trustworthy and Worrisome Websites
Understanding how misleading and outright false information enters news ecosystems remains a difficult challenge that requires tracking how narratives spread across thousands of fringe and mainstream news websites. To do this, we introduce a system that utilizes encoder-based large language models and zero-shot stance detection to scalably identify and track news narratives and their attitudes across over 4,000 factually unreliable, mixed-reliability, and factually reliable English-language news websites. Running our system over an 18 month period, we track the spread of 146K news stories. Using network-based interference via the NETINF algorithm, we show that the paths of news narratives and the stances of websites toward particular entities can be used to uncover slanted propaganda networks ({e.g.}, anti-vaccine and anti-Ukraine) and to identify the most influential websites in spreading these attitudes in the broader news ecosystem. We hope that increased visibility into our distributed news ecosystem can help with the reporting and fact-checking of propaganda and disinformation.

## Website and URL Information

We provide the domains and the URLs we utilized within this work. The domains can be found in the `domains.txt` and the URLS can be downloaded [here](https://drive.google.com/file/d/1OFibzqt2eQHBsbPU8KfKFteFib8DvSnG/view?usp=sharing).

### Unreliable News Websites
We collect articles from 1,003 websites labeled as having "low" or "very low" factual reporting by Media-Bias/Fact-Check. We extend this list with conspiracy theory-promoting websites identified by [Hanley et al](https://dl.acm.org/doi/10.1145/3610043). Our list of unreliable news websites includes pseudo-science sites like vaccine.news, state-propaganda outlets such as rt.com, and partisan websites with low-factuality ratings like the liberal-leaning occupydemocrats.com.

### Mixed-Reliability Websites
We collect articles from 1,012 mixed-reliability news websites labeled as having mixed factual reporting by Media-Bias/Fact-Check. This list includes websites across the political spectrum, such as foxnews.com, nypost.com, and theguardian.com.
 
### Reliable News Websites.
We collect articles from 2,061 reliable news websites labeled as having high, very high, or mostly factual reporting by Media-Bias/Fact-Check. The category "mostly factual" is included to capture sources with strong reputations like The Washington Post. This list features websites such as reuters.com and apnews.com.

## DP-Means Clustering

We utilize DP-Means clustering via cosine similarity to identify narratives/stories. A cosine similarity implementation can be found in the folder `dpmeans_clustering`.


## License and Copyright

Copyright 2025 The Board of Trustees of The Leland Stanford Junior University

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


