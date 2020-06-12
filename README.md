## Predictive Inference Task (online)

This repository contains code to run an predictive inference task adapted from [Vaghi et al. 2017](https://doi.org/10.1016/j.neuron.2017.09.006) for web-based testing. The online task was used for the study:

<strong>Seow, T. X.F.</strong> & Gillan, C. M. (2020). [Transdiagnostic phenotyping reveals a host of metacognitive deficits implicated in compulsivity.](https://www.nature.com/articles/s41598-020-59646-4) <i>Scientific Reports</i>, <strong>10</strong>(1), 1-11.

<p align="center">
  <img src="https://github.com/seowxft/predictive-inference-task-online/blob/master/images/task.tif" alt="TaskFig"/>
</p>

<strong>Predictive-inference task</strong>. (<strong>a</strong>) Trial sequence. Participants were instructed to position a bucket (yellow arc on the circle edge) to catch a flying particle, and thereafter rated their confidence that they would catch the particle. Particles were fired from the centre of the circle to the edge. Points were gained when the particle was caught, and the bucket turned green; else, points were lost and the bucket turned red. (<strong>b</strong>) Particle trajectories. For every trial, landing locations were independently sampled from a Gaussian distribution. As such, particles landed around the same area with small variations induced by noise. For illustration purposes, dashed arrow lines represent particle trajectory of current (black) and past (blue) trials, which over trials allow subjects to generate a representation of the Gaussian. (<strong>c</strong>) Change-points. The mean of the distribution abruptly moves to another point on the circle when a “change-point” occurs. This new mean is then sampled in the same manner as (<strong>b</strong>) until the next change-point.

Notes:
- This version has two hazard rate conditions that varied the number of change-points in a stretch of trials each, as opposed to one hazard rate in [Vaghi et al. 2017](https://doi.org/10.1016/j.neuron.2017.09.006).
- `data_buckPos` is recorded from the <i>edge</i> of the bucket. For analysis purposes, bucket position is measured from the <i>middle</i> of the bucket. Thus `<stim_bucketSize>/2` should be added to `data_buckPos` post-hoc.

## License
This work is licensed under the Creative Commons Attribution-Non Commercial 4.0 International (CC BY-NC 4.0). Feel free to use it and adapt it however you want for non-commerical purposes.

Copyright (c) 2020 Tricia Seow
