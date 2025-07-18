# LLMUsabilityEvaluations 

Data and code for our paper **Catching UX Flaws in Code: Leveraging LLMs to Identify Usability Flaws at the Development Stage**, as accepted to [VLHCC 2025](https://conf.researchr.org/home/vlhcc-2025).

## Methodology
The essence of this repository is to analyze usability evaluations conducted by Large Language Models (LLMs). 
For the paper mentioned above, we utilized a customized pipeline of OpenAI's ChatGPT-4o. The pipeline is [available here](https://chatgpt.com/g/g-680f8f4df7a88191b0efab9dd1d6a47b-vtcs-llm-usability-evaluations-research).
Our research methodology and process is thoroughly described in our paper. In short, the code in this repository:
- [x] steps through each folder in `/results`
- [x] analyzes the similarity and consistency of each of the three evaluations (`eval1.json`, `eval2.json`, `eval3.json`). 
- [x] calculates various IRR metrics for all of the data, including:
    - [x] Krippendorf's α
    - [x] Cohen's κ
    - [x] Fleiss' κ
- [x] Generates various tables and graphs based on this data.
- [x] Exports the generated graphs, for use in the paper.
- [x] Outputs the corresponding LaTeX equivalents of the tables, for use in the paper.

## Usage
If you would like to use our statistical analysis methods for your own usability research, feel free to. `analysis.ipynb` isn't written to only support our own research, and can easily be used to analyze your own results, provided you do so in a similar way. That is, organize all of your evaluation results (from the LLM) into `results/<repoName>`, with each folder containing `eval1.json`, `eval2.json`, and `eval3.json`. 


## Authors
1. [Nolan Platt](https://nolanplatt.com) | Virginia Tech Department of Computer Science
2. [Ethan Luchs](https://www.linkedin.com/in/ethanluchs) | Virginia Tech Department of Computer Science
3. [Dr. Sehrish Basir Nizamani](https://website.cs.vt.edu/people/faculty/sehrish-basir.html) | Assistant Professor, Virginia Tech Department of Computer Science

## Citation
Once officially published, the citation will be posted here. The paper will be available in the _Proceedings of the 2025 IEEE Symposium on Visual Languages and Human-Centric Computing (VL/HCC), 2025_


<p align="center">
<img src="static/vtcs.png" alt="Virginia Tech CS Logo" style="width:450px;height:82px;"> <br> <br>
<img src="static/chci.png" alt="CHCI Logo">

</p>
