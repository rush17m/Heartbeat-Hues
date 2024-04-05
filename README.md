# Heartbeat-Hues
Interpretability of time series data to better understand and visualize markers for Congestive Heart Failure

## Goal
The Project focuses on testing eXplainable AI (XAI) methods to try and help explain/understand some state-of-the-art models. We accomplish this by using LSTM and CNN Machine Learning Models to make accurate predictions about congestive heart failure using ECGs and explaining the Neural Network output/prediction using the LIMESegment, an XAI technique modified to work with time-series data.
<ul>
  <li> Recreating state-of-the-art models to detect congestive heart failure </li>
  <li> Implement XAI tools to explain time series data
        <ul>
          <li> LIMEsegment: The proposed adaptation of LIME to time series data of Sivill et al.: https://proceedings.mlr.press/v151/sivill22a.html </li>
          <li> Neves: The proposed adapatation of LIME to time series data of Neves et al.: https://boa.unimib.it/retrieve/handle/10281/324847/492202/Manuscript.pdf </li>
          <li> Leftist: The proposed adaptation of LIME to time series data of Guilleme et al.: https://ieeexplore.ieee.org/abstract/document/8995349
        </ul>
  </li> 
  <li> Generating explanations using chosen adaptation. </li>
</ul>

## Installation

<ul> 
  <li> Clone repository </li>
  <li> Install dependencies 'pip3 install -r requirements.txt' </li>
</ul>

## Content
<ul>
  <li> LimeSegment\Utils: 
    <ul> 
      <li> explanations.py: Contains code-generating explanations: 
        <ul>
          <li> LIMEsegment: Our proposed adaptation of LIME to time series data  </li>
          <li> Neves: The proposed adapatation of LIME to time series data of Neves et al.: https://boa.unimib.it/retrieve/handle/10281/324847/492202/Manuscript.pdf </li>
          <li> Leftist: The proposed adaptation of LIME to time series data of Guilleme et al.: https://ieeexplore.ieee.org/abstract/document/8995349
        </ul>
      <li> metrics.py: Contains code for the Robustness and Faithfulness measures used to evaluate each explanation module </li>
    </ul>
  </li>
  <li>download.ipynb: Code to download datasets from PhysioNet </li>
  <li>generate_cnn.ipynb: Code to train CNN based on work adapted by Porumb et al https://www.sciencedirect.com/science/article/abs/pii/S1746809419301776#bib0255</li>
  <li>lstm.ipynb: Code to train CNN based on work adapted by Wang et al https://www.mdpi.com/1424-8220/19/7/1502 </li>
  <li>explain.ipynb: Code to use pre-trained CNN and LSTM classifiers to generate explanations for predictions. Additional analysis was performed on the explanations. </li>
</ul>
