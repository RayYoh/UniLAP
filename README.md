# UniLAP: A Unified Latent Action Policy for Cross-Embodiment Manipulation

Project page: https://rayyoh.github.io/UniLAP/

The code release is in preparation and will land in this repository.

## Acknowledgements

UniLAP builds on many outstanding open-source projects and datasets. The dataset-derived
frames and simulator renders under `docs/` remain under their original licenses and terms;
the real-robot xArm7 footage and the figures are our own.

- **[NVIDIA DreamDojo](https://huggingface.co/nvidia/DreamDojo)**: the frozen, continuous
  LAM teacher that Stage I distills.
- **[NVIDIA Isaac GR00T](https://github.com/NVIDIA/Isaac-GR00T)**: the GR00T LeRobot data
  loader and the GR1 humanoid corpora used in Stage-I pretraining
  (`PhysicalAI-Robotics-GR00T-Teleop-GR1` and `PhysicalAI-Robotics-GR00T-X-Embodiment-Sim`).
- **[Apple EgoDex](https://github.com/apple/ml-egodex)**: the egocentric human video used in
  Stage-I pretraining and for the hand-pose forecasting benchmark.
- **[SimplerEnv](https://github.com/simpler-env/SimplerEnv)** and
  **[ManiSkill2-real2sim](https://github.com/simpler-env/ManiSkill2_real2sim)**: the simulated
  evaluation benchmark for the WidowX (Bridge) and Google Robot (Fractal) setups. The matching
  training data are **BridgeData V2** and the **RT-1** corpus (`fractal20220817_data`, Open
  X-Embodiment), used via the LeRobot v2.0 conversions from
  [IPEC-COMMUNITY](https://huggingface.co/IPEC-COMMUNITY).
- **[RoboCasa](https://github.com/robocasa/robocasa)** and
  **[robosuite](https://github.com/ARISE-Initiative/robosuite)**: the closed-loop evaluation
  environments for the GR1 humanoid tasks (via the
  [robocasa-gr1-tabletop-tasks](https://github.com/robocasa/robocasa-gr1-tabletop-tasks)
  suite); the RoboCasa365 pretrain split is also part of Stage-I co-training.
- **[LeRobot](https://github.com/huggingface/lerobot)**: the v2.0 dataset format used
  throughout.
- Frozen backbones: **[DINOv2](https://github.com/facebookresearch/dinov2)** (ViT-B/14),
  **SigLIP 2** (ViT-B/16), and **Flan-T5** (large).

## License

Released under the [MIT License](LICENSE). The MIT grant covers this repository's own
content; third-party datasets, simulators, pretrained models, and any third-party code
referenced above remain under their respective original licenses.
