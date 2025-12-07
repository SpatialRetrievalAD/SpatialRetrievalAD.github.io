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
paper: https://spatialretrievalad.github.io/
code: https://github.com/SpatialRetrievalAD/
data: https://huggingface.co/datasets/SpatialRetrievalAD/nuScenes-Geography-Data

---

<br>

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








<!-- Dataset Visualization -->
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






<!-- Quantitative Comparison -->
<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
    <div class="column is-four-fifths">
        <h2>Comparison</h2>
        <div class="content has-text-justified">
        </div>
    </div>
</div>



<!-- Generative World Model Results -->

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content has-text-justified">
      <p><strong>Generative World Model Results.</strong> Conditioning UniMLVG and MagicDriveDiT on geographic images leads to lower FVD and FID, effectively preventing scene drift and preserving geometric consistency during rollouts. This demonstrates that spatial retrieval provides a structural scaffold for coherent world modeling.</p>
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/result/result_generative.jpg" alt="generative" style="width: 65%;">
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/visualization/visualization_generative.jpg" alt="visualization_generative" style="width: 100%;">
    </div>
  </div>
</div>





<!-- Online Mapping Results -->

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content has-text-justified">
      <p><strong>Online Mapping Results.</strong> Integrating geographic priors into MapTR and MapTRv2 substantially improves online mapping. The extra background information enables recovery of occluded lanes.</p>
    </div>
  </div>
</div>


<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/result/result_mapping.jpg" alt="mapping" style="width: 100%;">
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/visualization/visualization_mapping.jpg" alt="visualization_mapping" style="width: 100%;">
    </div>
  </div>
</div>



<!-- Occupancy Results -->

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content has-text-justified">
      <p><strong>Occupancy Results.</strong> Extending FB-OCC and FlashOCC yields consistent mIoU improvements, particularly on static categories. The incorporation of geographic priors further boosts mIoU on static terrain, as they provide additional background information.</p>
    </div>
  </div>
</div>



<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content">
        <img src="./static/image/result/result_occupancy.jpg" alt="occupancy" style="width: 100%;">
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/visualization/visualization_occupancy.jpg" alt="visualization_occupancy" style="width: 100%;">
    </div>
  </div>
</div>




<!-- End-to-end Planning Results -->

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content has-text-justified">
      <p><strong>End-to-end Planning Results.</strong> We evaluate how spatial retrieval improves safe planning with VAD. Geographic priors provide stable road-layout information, compensating for sensing failures under occlusion or low light. With similar trajectory accuracy, our method achieves better safety margins, reducing the collision rate from 0.55% to 0.48% in challenging night scenes.</p>
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 0rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/result/result_planning.jpg" alt="planning" style="width: 100%;">
    </div>
  </div>
</div>

<div class="columns is-centered has-text-centered" style="margin-bottom: 3rem;">
  <div class="column is-four-fifths">
    <div class="content">
      <img src="./static/image/visualization/visualization_planning.jpg" alt="visualization_planning" style="width: 70%;">
    </div>
  </div>
</div>








<!-- Conclusion -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Conclusion</h2>
        <div class="content has-text-justified">
        &emsp;&emsp;In this work, we present the spatial retrieval paradigm for AD, introducing geographic data as an additional input. We extend nuScenes with geographic data by Google Maps APIs and evaluate five key AD tasks on the extended <a href="https://huggingface.co/datasets/SpatialRetrievalAD/nuScenes-Geography-Data" target="_blank">nuScenes-Geography</a>  dataset. We propose a general plug-and-play Spatial Retrieval Adapter module as an intuitive baseline to incorporate geographic data. We propose Reliability Estimation  to adaptively fuse geographic information based on the reliability of the retrieved data. Extensive experiments show that the proposed paradigm can enhance the performance of multiple AD tasks, demonstrating the substantial potential of the new paradigm.
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




