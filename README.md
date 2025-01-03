# Tracking the Takes and Trajectories of News Narratives from Trustworthy and Worrisome Websites
Uncovering and understanding how influence networks push propaganda and disinformation within the wider news ecosystem remains a difficult challenge that requires tracking and characterizing how narratives spread across thousands of fringe and mainstream news websites. Using 18 months of daily English-language news article scrapes from 1,003 unreliable news (e.g., twisted.news), 1,012 mixed-reliability websites (e.g., theepochtimes.com), and 2,061 reliable news websites (e.g., washingtonpost.com), the large language model E5, DP-Means clustering, and zero-shot stance detection, we develop a system to isolate and quantify the relationships between unreliable, mixed-reliability, and reliable news outlets. We show that by utilizing the stances of website articles toward particular entities and network inference-based tools, we can track slanted propaganda networks (e.g., anti-vaccine and anti-Ukraine) and identify the most influential websites in spreading particular attitudes, not only on fringe websites but within the broader media ecosystem, helping the reporting and fact-checking of propaganda and disinformation. 

## Website and URL Information

We provide the domains and the URLs we utilized within this work. The domains can be found in the `domains.txt` and the URLS can be downloaded [here]().

### Unreliable News Websites
We collect articles from 1,003 websites labeled as having "low" or "very low" factual reporting by Media-Bias/Fact-Check. We extend this list with conspiracy theory-promoting websites identified by Hanley et al.. Our list of unreliable news websites includes pseudo-science sites like vaccine.news, state-propaganda outlets such as rt.com, and partisan websites with low-factuality ratings like the liberal-leaning occupydemocrats.com.

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


