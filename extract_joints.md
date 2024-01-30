# How to extract joints?

```python
python -u training/train_rig.py --arch="jointnet_motion" -e --resume="checkpoints/jointnet_motion/model_best.pth.tar" --train_folder="YOUR_DATASET_PATH/train/" --val_folder="YOUR_DATASET_PATH/val/" --test_folder="YOUR_DATASET_PATH/test/" --output_folder="YOUR_OUTPUT_FOLDER"
python -u training/train_rig.py --arch="masknet_motion" -e --resume="checkpoints/masknet_motion/model_best.pth.tar" --train_folder="YOUR_DATASET_PATH/train/" --val_folder="YOUR_DATASET_PATH/val/" --test_folder="YOUR_DATASET_PATH/test/" --output_folder="YOUR_OUTPUT_FOLDER"
```