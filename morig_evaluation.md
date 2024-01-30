# Preparing Your Data

Make sure your mesh and any associated point cloud data are in a format that is compatible with the tools provided by MoRig. This might require preprocessing your data to match the expected input format of the scripts.

### Setup Environment

Ensure that you have the environment set up as described previously:

```bash
conda env create -f environment.yml
conda activate morig
```

### Testing & Evaluation

1. Output shifted points and their attention.
1. Prepare your data in a similar structure to what MoRig expects.
1. Potentially adapt the evaluation scripts to work with your dataset's specific format.
1. Ensure the pretrained models (if you're using them) are suitable for your data's characteristics, or train new models on your data.

#### Custom Steps

1. **Extract Joints**: Modify `eval_rigging.py` script if needed to correctly handle your data format and paths.
2. **Form Skeletons and Predict Skinning Weights**: Use modified versions of `pred_skel_func` and `pred_rig_func` within `joint2rig.py`, adjusting paths and potentially other parameters based on your dataset.
