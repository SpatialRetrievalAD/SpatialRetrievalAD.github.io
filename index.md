---
layout: project_page
permalink: /

title: |
  Spatial Retrieval Augmented
  Autonomous Driving

authors: |
  Xiaosong Jia<sup>1*</sup>, Chenhe Zhang<sup>1*</sup>, Yule Jiang<sup>2*</sup>, Songbur Wong<sup>2*</sup>,<br>
  Zhiyuan Zhang<sup>2</sup>, Chen Chen<sup>3</sup>, Shaofeng Zhang<sup>4</sup>, Xuanhe Zhou<sup>2</sup>, Xue Yang<sup>2†</sup>,<br>
  Junchi Yan<sup>2†</sup>, Yu-Gang Jiang<sup>1</sup><br>
  <small><sup>*</sup>Equal contributions &nbsp; <sup>†</sup>Correspondence authors</small>
affiliations: |
  <sup>1</sup>Institute of Trustworthy Embodied AI, Fudan University<br>
  <sup>2</sup>Shanghai Jiao Tong University<br>
  <sup>3</sup>Key Laboratory of Target Cognition and Application Technology, Aerospace Information Research Institute, Chinese Academy of Sciences<br>
  <sup>4</sup>University of Science and Technology of China
paper: https://aaa
# video: https://aaa
code: https://github.com/SpatialRetrievalAD/
data: https://huggingface.co/datasets/SpatialRetrievalAD/nuScenes-Geography-Data

---

<div class="columns is-centered has-text-centered video-container">
  <div class="column is-four-fifths">
    <!-- <h2>SpatialRetrievalAD Summary Video</h2> -->
    <div class="content">
      <video width="100%" controls>
        <source src="./static/video/demo.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
  </div>
</div>




<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
&emsp;&emsp;Existing autonomous driving systems rely on onboard sensors (cameras, LiDAR, IMU, etc) for environmental perception. However, this paradigm is limited by the drive-time perception horizon and often fails under limited view scope, occlusion or extreme conditions such as darkness and rain. In contrast, human drivers are able to recall road structure even under poor visibility. To endow models with this "recall" ability, we propose the spatial retrieval paradigm, introducing offline retrieved geographic images as an additional input. These images are easy to obtain from offline caches (e.g, Google Maps or stored autonomous driving datasets) without requiring additional sensors, making it a plug-and-play extension for existing AD tasks.
<br>
&emsp;&emsp;For experiments, we first extend the nuScenes dataset with geographic images retrieved via Google Maps APIs and align the new data with ego-vehicle trajectories. We establish baselines across five core autonomous driving tasks: object detection, online mapping, occupancy prediction, end-to-end planning, and generative world modeling.  Extensive experiments show that the extended modality could enhance the performance of certain tasks. We will open-source dataset curation code, data, and benchmarks for further study of this new autonomous driving paradigm.
        </div>
    </div>
</div>


<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/teaser.jpg" alt="teaser" style="width: 100%;">
    </div>
  </div>
</div>




<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>nuScenes-Geography Dataset</h2>
        <div class="content has-text-justified">
        &emsp;&emsp;We extend the nuScenes dataset with geographic images retrieved via Google Maps APIs and align the new data with ego-vehicle trajectories. 
        <br>
        &emsp;&emsp;The dataset and development toolkit are publicly available:
        <ul style="margin-top: 0.5em; margin-bottom: 0.5em;">
            <li><strong>Dataset:</strong> <a href="https://huggingface.co/datasets/SpatialRetrievalAD/nuScenes-Geography-Data" target="_blank">nuScenes-Geography-Data</a> on Hugging Face</li>
            <li><strong>Devkit:</strong> <a href="https://github.com/SpatialRetrievalAD/SpatialRetrievalAD-Dataset-Devkit" target="_blank">SpatialRetrievalAD-Dataset-Devkit</a> on GitHub</li>
        </ul>
        </div>
    </div>
</div>


<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/distribution.jpg" alt="distribution" style="width: 100%;">
    </div>
  </div>
</div>




<!-- Multi Tasks -->
<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
    <div class="column is-four-fifths">
        <h2>Task Baselines</h2>
        <div class="content has-text-justified">
        &emsp;&emsp;To systematically investigate the spatial retrieval paradigm, we establish baselines across five key AD tasks: object detection, online mapping, occupancy prediction, end-to-end planning, and generative world modeling. We design a plug-and-play adapter to seamlessly integrate geographic images into existing models. Extensive experiments demonstrate this modality improves performance across tasks. All implementation repositories are hosted under the 
        <a href="https://github.com/SpatialRetrievalAD" target="_blank">SpatialRetrievalAD</a> organization:
        </div>
        <div class="content" style="margin-top: 1.5rem;">
            <table class="table is-striped is-fullwidth" style="margin: 0 auto;">
                <thead>
                    <tr>
                        <th style="text-align: left; padding: 0.75em;">Task</th>
                        <th style="text-align: center; padding: 0.75em;">Repository</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td style="text-align: left; padding: 0.75em;"><strong>Generative World Modeling</strong></td>
                        <td style="text-align: center; padding: 0.75em;">
                            <a href="https://github.com/SpatialRetrievalAD/Generative-World-Model" target="_blank">Generative-World-Model</a> 
                        </td>
                    </tr>
                    <tr>
                        <td style="text-align: left; padding: 0.75em;"><strong>End-to-End Planning</strong></td>
                        <td style="text-align: center; padding: 0.75em;">
                            <a href="https://github.com/SpatialRetrievalAD/End2End-Planning" target="_blank">End2End-Planning</a>
                        </td>
                    </tr>
                    <tr>
                        <td style="text-align: left; padding: 0.75em;"><strong>Online Mapping</strong></td>
                        <td style="text-align: center; padding: 0.75em;">
                            <a href="https://github.com/SpatialRetrievalAD/Online-Mapping" target="_blank">Online-Mapping</a>
                        </td>
                    </tr>
                    <tr>
                        <td style="text-align: left; padding: 0.75em;"><strong>Occupancy Prediction</strong></td>
                        <td style="text-align: center; padding: 0.75em;">
                            <a href="https://github.com/SpatialRetrievalAD/Occupancy-Prediction" target="_blank">Occupancy-Prediction</a>
                        </td>
                    </tr>
                    <tr>
                        <td style="text-align: left; padding: 0.75em;"><strong>Object Detection</strong></td>
                        <td style="text-align: center; padding: 0.75em;">
                            <a href="https://github.com/SpatialRetrievalAD/3D-Detection" target="_blank">3D-Detection</a>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</div>




<!-- Data Example -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Dataset Visualization</h2>
        <div class="content has-text-justified">
        The following figures show the correspondence between Geography images and nuScenes images:
        </div>
    </div>
</div>


<div class="columns is-centered has-text-centered" style="margin-bottom: -1.5rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/data_example_0.jpg" alt="data_example_0" style="width: 100%;">
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: -1.5rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/data_example_1.jpg" alt="data_example_1" style="width: 100%;">
    </div>
  </div>
</div>


<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
        <img src="./static/image/data_example_2.jpg" alt="data_example_2" style="width: 100%;">
    </div>
  </div>
</div>

<!-- Citation Section -->
<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
    <div class="column is-four-fifths">
        <h2>Citation</h2>
        <div class="content">
            <p>If you use SpatialRetrievalAD in your research, please cite our paper:</p>
            <pre><code>
</code></pre>
        </div>
    </div>
</div>







<!-- Acknowledgments Section -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Acknowledgments</h2>
        <div class="content">
            <p>We thank the following projects for their contributions to the development of this project:
                <a href="https://github.com/HuangJunJie2017/BEVDet" target="_blank">BEVDet</a>, 
                <a href="https://github.com/fundamentalvision/BEVFormer" target="_blank">BEVFormer</a>, 
                <a href="https://github.com/NVlabs/FB-BEV" target="_blank">FB-OCC</a>, 
                <a href="https://github.com/Yzichen/FlashOCC" target="_blank">FlashOCC</a>, 
                <a href="https://github.com/flymin/MagicDrive-V2" target="_blank">MagicDriveDiT</a>, 
                <a href="https://github.com/hustvl/MapTR" target="_blank">MapTR</a>, 
                <a href="https://github.com/hustvl/MapTR/tree/maptrv2" target="_blank">MapTRv2</a>, 
                <a href="https://www.nuscenes.org/" target="_blank">nuScenes</a>, 
                <a href="https://github.com/megvii-research/PETR" target="_blank">PETR</a>, 
                <a href="https://github.com/SenseTime-FVG/OpenDWM" target="_blank">UniMLVG</a>, 
                <a href="https://github.com/hustvl/VAD" target="_blank">VAD</a>
            </p>
        </div>
    </div>
</div>








<!-- > Note: This is an example of a Jekyll-based project website template: [Github link](https://github.com/shunzh/project_website).\
> The following content is generated by ChatGPT. The figure is manually added. -->

<!-- ## Background
The paper "On Computable Numbers, with an Application to the Entscheidungsproblem" was published by Alan Turing in 1936. In this groundbreaking paper, Turing introduced the concept of a universal computing machine, now known as the Turing machine.

## Objective
Turing's main objective in this paper was to investigate the notion of computability and its relation to the Entscheidungsproblem (the decision problem), which is concerned with determining whether a given mathematical statement is provable or not.


## Key Ideas
1. Turing first presented the concept of a "computable number," which refers to a number that can be computed by an algorithm or a definite step-by-step process.
2. He introduced the notion of a Turing machine, an abstract computational device consisting of an infinite tape divided into cells and a read-write head. The machine can read and write symbols on the tape, move the head left or right, and transition between states based on a set of rules.
3. Turing demonstrated that the set of computable numbers is enumerable, meaning it can be listed in a systematic way, even though it is not necessarily countable.
4. He proved the existence of non-computable numbers, which cannot be computed by any Turing machine.
5. Turing showed that the Entscheidungsproblem is undecidable, meaning there is no algorithm that can determine, for any given mathematical statement, whether it is provable or not.

![Turing Machine](/static/image/Turing_machine.png)

*Figure 1: A representation of a Turing Machine. Source: [Wiki](https://en.wikipedia.org/wiki/Turing_machine).*

## Table: Comparison of Computable and Non-Computable Numbers

| Computable Numbers | Non-Computable Numbers |
|-------------------|-----------------------|
| Rational numbers, e.g., 1/2, 3/4 | Transcendental numbers, e.g., π, e |
| Algebraic numbers, e.g., √2, ∛3 | Non-algebraic numbers, e.g., √2 + √3 |
| Numbers with finite decimal representations | Numbers with infinite, non-repeating decimal representations |

He used the concept of a universal Turing machine to prove that the set of computable functions is recursively enumerable, meaning it can be listed by an algorithm.

## Significance
Turing's paper laid the foundation for the theory of computation and had a profound impact on the development of computer science. The Turing machine became a fundamental concept in theoretical computer science, serving as a theoretical model for studying the limits and capabilities of computation. Turing's work also influenced the development of programming languages, algorithms, and the design of modern computers.

## Citation
```

``` -->
