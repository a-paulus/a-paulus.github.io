<p>
I am a PhD student with the IMPRS-IS program at the University of Tuebingen and the Max-Planck-Institute for Intelligent Systems, supervised by <a href="https://uni-tuebingen.de/en/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/distributed-intelligence/team/prof-dr-georg-martius/">Georg Martius</a>.
I am interested in <b>differentiable and amortized optimization, LLM safety and reasoning</b>.
Currently I am interning in the
<b>Fundamental AI Research (FAIR)</b>
group at
<b>Meta</b> in Menlo Park, where I study LLM safety from a game-theoretical perspective, supervised by <a href="https://arman-z.github.io">Arman Zharmagambetov</a>.

A few major themes of my research involve:
</p>

<ol>
<li>
  <b>attacking language models</b> to improve safety and alignment
  (in <a href="https://arxiv.org/abs/2404.16873">AdvPrompter</a>)
</li>
<li>
  <b>differentiable combinatorial optimization</b>
  (in
  <a href="https://arxiv.org/abs/1912.02175">blackbox solver differentiation</a>,
  <a href="https://arxiv.org/abs/2105.02343">CombOptNet</a>, and
  <a href="https://arxiv.org/abs/2407.05920v1">LPGD</a>)
</li>
<li>
  <b>differentiable physics simulation</b>
  (in
  <a href="https://arxiv.org/abs/2506.14186">DiffMJX</a>)
</li>
</ol>
<br>


## <i class="fa fa-chevron-right"></i> Education

<table class="table table-hover">
  <tr>
    <td>
      <span class='cvdate'>2021&nbsp;-&nbsp;2022</span>
      <strong>M.Sc. in Computer Science</strong>, <em>University of Tuebingen</em>
        (4.00/4.00)
      <br>
    </td>
  </tr>
  <tr>
    <td>
      <span class='cvdate'>2018&nbsp;-&nbsp;2021</span>
      <strong>B.S. in Computer Science</strong>, <em>University of Tuebingen</em>
        (3.73/4.00)
      <br>
    </td>
  </tr>
  <tr>
    <td>
      <span class='cvdate'>2015&nbsp;-&nbsp;2021</span>
      <strong>B.S. in Physics</strong>, <em>University of Tuebingen</em>
        (3.80/4.00)
      <br>
    </td>
  </tr>
</table>


## <i class="fa fa-chevron-right"></i> Previous Positions
<table class="table table-hover">
<tr>
  <td style='padding-right:0;'>
<span class='cvdate'>2023&nbsp;-&nbsp;2024</span>
<p markdown="1" style='margin: 0'><strong>Research Scientist Intern</strong>, <em>Meta, Fundamental AI Research (FAIR)</em>, New York City
<span markdown="1" style="color:grey;font-size:1.3rem;margin: 0">
(with <a href="https://bamos.github.io" target="_blank">Brandon Amos</a> on amortized optimization for LLM safety)
</span></p>
  </td>
</tr>
<tr>
  <td style='padding-right:0;'>
<span class='cvdate'>2016&nbsp;-&nbsp;2019</span>
<p markdown="1" style='margin: 0'><strong>Research Assistant</strong>, <em>Max-Planck-Institute for Intelligent Systems</em>, Tuebingen, Germany
<span markdown="1" style="color:grey;font-size:1.3rem;margin: 0">
(with <a href="https://uni-tuebingen.de/en/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/distributed-intelligence/team/prof-dr-georg-martius/" target="_blank">Georg Martius</a> on differentiable combinatorial optimization)
</span></p>
  </td>
</tr>
</table>


## <i class="fa fa-chevron-right"></i> Publications

<!-- I usually publish at machine learning conferences, -->
<!-- including . -->
<!-- <a href="https://scholar.google.com/citations?user=njZL5CQAAAAJ">Google Scholar</a> -->
<!-- reports 0.9k+ citations and an h-index of 6. -->
<!-- The selected publications I am a primary author on are <span style='background-color: #ffffd0'>highlighted.</span> -->

<!-- [<a href="https://scholar.google.com/citations?user=njZL5CQAAAAJ">Google Scholar</a>: 0.9k+ citations and an h-index of 6] <br> -->
[<a href="https://scholar.google.com/citations?user=njZL5CQAAAAJ">Google Scholar</a>: 0.9k+ citations] <br>
Selected publications I am a primary author on are <span style='background-color: #ffffd0'>highlighted.</span>

<h2>2025</h2>
<table class="table table-hover">

<tr id="tr-paulus2025advprompter" style="background-color: #ffffd0">
<td align='right' style='padding-left:0;padding-right:0;'>
1.
</td>
<td>
<a href='https://arxiv.org/abs/2404.16873' target='_blank'><img src="images/publications/paulus2025advprompter.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/abs/2404.16873' target='_blank'>AdvPrompter: Fast Adaptive Adversarial Prompting for LLMs</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_paulus2025advprompter").toggle()'>abs</a>] [<a href='https://github.com/facebookresearch/advprompter' target='_blank'>code</a>] <br>
<strong>Anselm&nbsp;Paulus*</strong>, <a href='https://arman-z.github.io/' target='_blank'>Arman&nbsp;Zharmagambetov*</a>, <a href='https://sites.google.com/view/chuanguo' target='_blank'>Chuan&nbsp;Guo</a>, <a href='https://bamos.github.io/' target='_blank'>Brandon&nbsp;Amos<sup>&dagger;</sup></a>, and <a href='https://yuandong-tian.com' target='_blank'>Yuandong&nbsp;Tian<sup>&dagger;</sup></a><br>
ICML 2025  <br>

<div id="abs_paulus2025advprompter" style="text-align: justify; display: none" markdown="1">
Large Language Models (LLMs) are vulnerable to jailbreaking attacks that lead to generation of inappropriate or harmful content. Manual red-teaming requires a time-consuming search for adversarial prompts, whereas automatic adversarial prompt generation often leads to semantically meaningless attacks that do not scale well. In this paper, we present a novel method that uses another LLM, called AdvPrompter, to generate human-readable adversarial prompts in seconds. AdvPrompter, which is trained using an alternating optimization algorithm, generates suffixes that veil the input instruction without changing its meaning, such that the TargetLLM is lured to give a harmful response. Experimental results on popular open source TargetLLMs show highly competitive results on the AdvBench and HarmBench datasets, that also transfer to closed-source black-box LLMs. We also show that training on adversarial suffixes generated by AdvPrompter is a promising strategy for improving the robustness of LLMs to jailbreaking attacks.
</div>

</td>
</tr>


<tr id="tr-paulus2025hard" style="background-color: #ffffd0">
<td align='right' style='padding-left:0;padding-right:0;'>
2.
</td>
<td>
<a href='https://arxiv.org/abs/2506.14186' target='_blank'><img src="images/publications/paulus2025hard.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/abs/2506.14186' target='_blank'>Hard Contacts with Soft Gradients: Refining Differentiable Simulators for Learning and Control</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_paulus2025hard").toggle()'>abs</a>]<br>
<strong>Anselm&nbsp;Paulus*</strong>, <a href='https://andregeist.github.io' target='_blank'>Andreas&nbsp;René&nbsp;Geist*</a>, <a href='https://p-schumacher.github.io' target='_blank'>Pierre&nbsp;Schumacher</a>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a>, and <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a><br>
Under submission 2025  <br>

<div id="abs_paulus2025hard" style="text-align: justify; display: none" markdown="1">
Contact forces pose a major challenge for gradient-based optimization of robot dynamics as they introduce jumps in the system's velocities. Penalty-based simulators, such as MuJoCo, simplify gradient computation by softening the contact forces. However, realistically simulating hard contacts requires very stiff contact settings, which leads to incorrect gradients when using automatic differentiation. On the other hand, using non-stiff settings strongly increases the sim-to-real gap. We analyze the contact computation of penalty-based simulators to identify the causes of gradient errors. Then, we propose DiffMJX, which combines adaptive integration with MuJoCo XLA, to notably improve gradient quality in the presence of hard contacts. Finally, we address a key limitation of contact gradients: they vanish when objects do not touch. To overcome this, we introduce Contacts From Distance (CFD), a mechanism that enables the simulator to generate informative contact gradients even before objects are in contact. To preserve physical realism, we apply CFD only in the backward pass using a straight-through trick, allowing us to compute useful gradients without modifying the forward simulation.
</div>

</td>
</tr>

</table>
<h2>2024</h2>
<table class="table table-hover">

<tr id="tr-paulus2024lpgd" style="background-color: #ffffd0">
<td align='right' style='padding-left:0;padding-right:0;'>
3.
</td>
<td>
<a href='https://arxiv.org/abs/2407.05920' target='_blank'><img src="images/publications/paulus2024lpgd.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/abs/2407.05920' target='_blank'>LPGD: A General Framework for Backpropagation through Embedded Optimization Layers</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_paulus2024lpgd").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/diffcp-lpgd' target='_blank'>code</a>] <br>
<strong>Anselm&nbsp;Paulus</strong>, <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a>, and <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a><br>
ICML 2024  <br>

<div id="abs_paulus2024lpgd" style="text-align: justify; display: none" markdown="1">
Embedding parameterized optimization problems as layers into machine learning architectures serves as a powerful inductive bias. Training such architectures with stochastic gradient descent requires care, as degenerate derivatives of the embedded optimization problem often render the gradients uninformative. We propose Lagrangian Proximal Gradient Descent (LPGD) a flexible framework for training architectures with embedded optimization layers that seamlessly integrates into automatic differentiation libraries. LPGD efficiently computes meaningful replacements of the degenerate optimization layer derivatives by re-running the forward solver oracle on a perturbed input. LPGD captures various previously proposed methods as special cases, while fostering deep links to traditional optimization methods. We theoretically analyze our method and demonstrate on historical and synthetic data that LPGD converges faster than gradient descent even in a differentiable setup.
</div>

</td>
</tr>

</table>
<h2>2023</h2>
<table class="table table-hover">

<tr id="tr-sahoo2024gradient" >
<td align='right' style='padding-left:0;padding-right:0;'>
4.
</td>
<td>
<a href='https://arxiv.org/abs/2205.15213' target='_blank'><img src="images/publications/sahoo2024gradient.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/abs/2205.15213' target='_blank'>Backpropagation through Combinatorial Algorithms: Identity with Projection Works</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_sahoo2024gradient").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/solver-differentiation-identity' target='_blank'>code</a>] <br>
<strong>Anselm&nbsp;Paulus*</strong>, <a href='https://s-sahoo.com' target='_blank'>Subham&nbsp;Sekhar&nbsp;Sahoo*</a>, <a href='https://jimimvp.github.io' target='_blank'>Marin&nbsp;Vlastelica</a>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a>, <a href='https://scholar.google.com/citations?user=RY_t8XAAAAAJ' target='_blank'>Volodymyr&nbsp;Kuleshov</a>, and <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a><br>
ICLR 2023  <br>

<div id="abs_sahoo2024gradient" style="text-align: justify; display: none" markdown="1">
Embedding discrete solvers as differentiable layers has given modern deep learning architectures combinatorial expressivity and discrete reasoning capabilities. The derivative of these solvers is zero or undefined, therefore a meaningful replacement is crucial for effective gradient-based learning. Prior works rely on smoothing the solver with input perturbations, relaxing the solver to continuous problems, or interpolating the loss landscape with techniques that typically require additional solver calls, introduce extra hyper-parameters, or compromise performance. We propose a principled approach to exploit the geometry of the discrete solution space to treat the solver as a negative identity on the backward pass and further provide a theoretical justification. Our experiments demonstrate that such a straightforward hyper-parameter-free approach is able to compete with previous more complex methods on numerous experiments such as backpropagation through discrete samplers, deep graph matching, and image retrieval. Furthermore, we substitute the previously proposed problem-specific and label-dependent margin with a generic regularization procedure that prevents cost collapse and increases robustness.
</div>

</td>
</tr>

</table>
<h2>2021</h2>
<table class="table table-hover">

<tr id="tr-paulus2021comboptnet" >
<td align='right' style='padding-left:0;padding-right:0;'>
5.
</td>
<td>
<a href='https://arxiv.org/pdf/2105.02343' target='_blank'><img src="images/publications/paulus2021comboptnet.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/pdf/2105.02343' target='_blank'>CombOptNet: Fit the Right NP-Hard Problem by Learning Integer Programming Constraints</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_paulus2021comboptnet").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/CombOptNet' target='_blank'>code</a>] <br>
<strong>Anselm&nbsp;Paulus</strong>, <a href='https://mrolinek.github.io/' target='_blank'>Michal&nbsp;Rolínek</a>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a>, <a href='https://bamos.github.io/' target='_blank'>Brandon&nbsp;Amos</a>, and <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a><br>
ICML 2021 (Spotlight, Oral at LMCA NeurIPS 2020 workshop) <br>

<div id="abs_paulus2021comboptnet" style="text-align: justify; display: none" markdown="1">
Bridging logical and algorithmic reasoning with modern machine learning techniques is a fundamental challenge with potentially transformative impact. On the algorithmic side, many NP-hard problems can be expressed as integer programs, in which the constraints play the role of their "combinatorial specification." In this work, we aim to integrate integer programming solvers into neural network architectures as layers capable of learning both the cost terms and the constraints. The resulting end-to-end trainable architectures jointly extract features from raw data and solve a suitable (learned) combinatorial problem with state-of-the-art integer programming solvers. We demonstrate the potential of such layers with an extensive performance analysis on synthetic data and with a demonstration on a competitive computer vision keypoint matching benchmark.
</div>

</td>
</tr>

</table>
<h2>2020</h2>
<table class="table table-hover">

<tr id="tr-vlastelica2020differentiation" style="background-color: #ffffd0">
<td align='right' style='padding-left:0;padding-right:0;'>
6.
</td>
<td>
<a href='http://arxiv.org/abs/1912.02175' target='_blank'><img src="images/publications/vlastelica2020differentiation.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='http://arxiv.org/abs/1912.02175' target='_blank'>Differentiation of Blackbox Combinatorial Solvers</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_vlastelica2020differentiation").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/blackbox-backprop' target='_blank'>code</a>] <br>
<strong>Anselm&nbsp;Paulus*</strong>, <a href='https://jimimvp.github.io' target='_blank'>Marin&nbsp;Vlastelica&nbsp;P.*</a>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a>, <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a>, and <a href='https://mrolinek.github.io/' target='_blank'>Michal&nbsp;Rolínek</a><br>
ICLR 2020 (Spotlight) <br>

<div id="abs_vlastelica2020differentiation" style="text-align: justify; display: none" markdown="1">
Achieving fusion of deep learning with combinatorial algorithms promises transformative changes to artificial intelligence. One possible approach is to introduce combinatorial building blocks into neural networks. Such end-to-end architectures have the potential to tackle combinatorial problems on raw input data such as ensuring global consistency in multi-object tracking or route planning on maps in robotics. In this work, we present a method that implements an efficient backward pass through blackbox implementations of combinatorial solvers with linear objective functions. We provide both theoretical and experimental backing. In particular, we incorporate the Gurobi MIP solver, Blossom V algorithm, and Dijkstra's algorithm into architectures that extract suitable features from raw inputs for the traveling salesman problem, the min-cost perfect matching problem and the shortest path problem.
</div>

</td>
</tr>


<tr id="tr-rolinek2020optimizing" >
<td align='right' style='padding-left:0;padding-right:0;'>
7.
</td>
<td>
<a href='http://arxiv.org/abs/1912.03500' target='_blank'><img src="images/publications/rolinek2020optimizing.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='http://arxiv.org/abs/1912.03500' target='_blank'>Optimizing Rank-based Metrics with Blackbox Differentiation</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_rolinek2020optimizing").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/blackbox-backprop' target='_blank'>code</a>] <br>
<a href='https://mrolinek.github.io/' target='_blank'>Michal&nbsp;Rolínek*</a>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil*</a>, <strong>Anselm&nbsp;Paulus</strong>, <a href='https://jimimvp.github.io' target='_blank'>Marin&nbsp;Vlastelica&nbsp;P.</a>, <a href='https://scholar.google.com/citations?user=ORqsx1YAAAAJ' target='_blank'>Claudio&nbsp;Michaelis</a>, and <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a><br>
CVPR 2020 (Oral, best paper award nomination) <br>

<div id="abs_rolinek2020optimizing" style="text-align: justify; display: none" markdown="1">
Rank-based metrics are some of the most widely used criteria for performance evaluation of computer vision models. Despite years of effort, direct optimization for these metrics remains a challenge due to their non-differentiable and non-decomposable nature. We present an efficient, theoretically sound, and general method for differentiating rank-based metrics with mini-batch gradient descent. In addition, we address optimization instability and sparsity of the supervision signal that both arise from using rank-based metrics as optimization targets. Resulting losses based on recall and Average Precision are applied to image retrieval and object detection tasks. We obtain performance that is competitive with state-of-the-art on standard image retrieval datasets and consistently improve performance of near state-of-the-art object detectors.
</div>

</td>
</tr>


<tr id="tr-rolinek2020deepgraphmatching" >
<td align='right' style='padding-left:0;padding-right:0;'>
8.
</td>
<td>
<a href='https://arxiv.org/abs/2003.11657' target='_blank'><img src="images/publications/rolinek2020deepgraphmatching.png" onerror="this.style.display='none'" class="publicationImg" /></a> 
<em><a href='https://arxiv.org/abs/2003.11657' target='_blank'>Deep Graph Matching via Blackbox Differentiation of Combinatorial Solvers</a> </em> 
[<a href='javascript:;'
    onclick='$("#abs_rolinek2020deepgraphmatching").toggle()'>abs</a>] [<a href='https://github.com/martius-lab/blackbox-deep-graph-matching' target='_blank'>code</a>] <br>
<a href='https://mrolinek.github.io/' target='_blank'>Michal&nbsp;Rolínek</a>, <a href='https://scholar.google.com/citations?user=hSQ7TbMAAAAJ' target='_blank'>Paul&nbsp;Swoboda</a>, <a href='https://scholar.google.com/citations?user=jkIx0f8AAAAJ' target='_blank'>Dominik&nbsp;Zietlow</a>, <strong>Anselm&nbsp;Paulus</strong>, <a href='https://scholar.google.com/citations?user=hA1rlU4AAAAJ' target='_blank'>Vít&nbsp;Musil</a>, and <a href='https://scholar.google.com/citations?user=b-JF-UIAAAAJ' target='_blank'>Georg&nbsp;Martius</a><br>
ECCV 2020  <br>

<div id="abs_rolinek2020deepgraphmatching" style="text-align: justify; display: none" markdown="1">
Building on recent progress at the intersection of combinatorial optimization and deep learning, we propose an end-to-end trainable architecture for deep graph matching that contains unmodified combinatorial solvers. Using the presence of heavily optimized combinatorial solvers together with some improvements in architecture design, we advance state-of-the-art on deep graph matching benchmarks for keypoint correspondence. In addition, we highlight the conceptual advantages of incorporating solvers into deep learning architectures, such as the possibility of post-processing with a strong multi-graph matching solver or the indifference to changes in the training setting. Finally, we propose two new challenging experimental setups.
</div>

</td>
</tr>

</table>


## <i class="fa fa-chevron-right"></i> Open Source Repositories
0.6k+ GitHub stars across all repositories.

<table class="table table-hover">
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>1.</td>
  <td>
    <span class='cvdate'>2025</span>
    <a href="https://github.com/facebookresearch/advprompter">facebookresearch/advprompter</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;162 |
    </span>
    <em>AdvPrompter (Adversarial attacks on LLMs)</em>
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>2.</td>
  <td>
    <span class='cvdate'>2024</span>
    <a href="https://github.com/martius-lab/diffcp-lpgd">martius-lab/diffcp-lpgd</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;2 |
    </span>
    <em>Lagrangian Proximal Gradient Descent (now merged into <a href="https://github.com/cvxpy/cvxpy" target="_blank">CVXPY</a>)</em>
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>3.</td>
  <td>
    <span class='cvdate'>2023</span>
    <a href="https://github.com/martius-lab/solver-differentiation-identity">martius-lab/solver-differentiation-identity</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;10 |
    </span>
    <em>Blackbox Identity Differentiation</em>
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>4.</td>
  <td>
    <span class='cvdate'>2021</span>
    <a href="https://github.com/martius-lab/CombOptNet">martius-lab/CombOptNet</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;72 |
    </span>
    <em>CombOptNet</em>
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>5.</td>
  <td>
    <span class='cvdate'>2020</span>
    <a href="https://github.com/martius-lab/blackbox-deep-graph-matching">martius-lab/blackbox-deep-graph-matching</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;88 |
    </span>
    <em>Deep Graph Matching</em>
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>6.</td>
  <td>
    <span class='cvdate'>2020</span>
    <a href="https://github.com/martius-lab/blackbox-backprop">martius-lab/blackbox-backprop</a>
    <span style="white-space: nowrap">
    | <i class="fa fas fa-star"></i>&nbsp;346 |
    </span>
    <em>Blackbox Differentiation</em>
  </td>
</tr>
</table>


## <i class="fa fa-chevron-right"></i> Invited Talks
<!-- Slides for my major presentations are available
[here](https://bamos.github.io/presentations/)
under a CC-BY license. -->

<table class="table table-hover">
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>1.</td>
  <td style='padding-right:0;'>
    <span class='cvdate'>2024</span>
     <em>AdvPrompter: Fast Adaptive Adversarial Prompting for LLMs</em> &mdash;
        Masaryk University, Brno, Czechia
  </td>
</tr>
<tr>
  <td align='right' style='padding-right:0;padding-left:0;'>2.</td>
  <td style='padding-right:0;'>
    <span class='cvdate'>2022</span>
     <em>On differentiable combinatorial optimization</em> &mdash;
        <a href="https://www.dagstuhl.de/de/seminars/seminar-calendar/seminar-details/22291">Dagstuhl Seminar: Machine Learning and Logical Reasoning: The New Frontier</a>
  </td>
</tr>
</table>


## <i class="fa fa-chevron-right"></i> Professional Activities
<table class="table table-hover">
</table>

### Reviewing
<table class="table table-hover">
<tr>
  <td style='padding-right:0;'>International Conference on Learning Representations (ICLR): 2022, 2023, 2024, 2025</td>
</tr>
<tr>
  <td style='padding-right:0;'>International Conference on Machine Learning (ICML): 2022, 2023, 2024, 2025</td>
</tr>
<tr>
  <td style='padding-right:0;'>Neural Information Processing Systems (NeurIPS): 2021, 2022, 2025</td>
</tr>
<tr>
  <td style='padding-right:0;'>Neural Information Processing Systems (NeurIPS) DiffCoAlg Workshop: 2025</td>
</tr>
</table>


## <i class="fa fa-chevron-right"></i> Skills
<table class="table table-hover">
<tr>
  <td class='col-md-2'>Programming</td>
  <td>
C++, Java, Python
  </td>
</tr>
<tr>
  <td class='col-md-2'>Frameworks</td>
  <td>
JAX, NumPy, Pandas, PyTorch, SciPy, TensorFlow
  </td>
</tr>
<tr>
  <td class='col-md-2'>Toolbox</td>
  <td>
Linux, emacs, git, tmux, zsh, uv, vscode
  </td>
</tr>
</table>
