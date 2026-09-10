# EfficientSAM Tests

This notebook compares the segmentation quality and robustness of **EfficientSAM-Ti**, **EfficientSAM-S**, and **SAM**.

## Requirements

- Python
- VS Code with the **Python** and **Jupyter** extensions
- The required Python packages:

```bash
pip install torch torchvision numpy matplotlib pillow fiftyone segment-anything
```

Download the [SAM ViT-H checkpoint](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth) and place it here:

```text
EfficientSAM/checkpoints/sam_vit_h_4b8939.pth
```

## Run the tests

Open `EfficientSAM_example.ipynb` in VS Code (or your favourite notebook IDE), select the correct Python interpreter, and click **Run All**.

## Included tests

- **Box prompts** - compares segmentation IoU using bounding-box prompts
- **Point prompts** - compares segmentation IoU using point prompts
- **Gaussian noise** - measures robustness as image noise increases
- **Shifted boxes** - measures robustness to inaccurate box prompts
- **Best and worst examples** - visualizes selected segmentation results
- **Inference time** - compares the models' average execution time
