## Getting Started

### Training

Run `python train.py [config-file]`, for example:

```
# Student  model
python train_final.py
```

Explanation of some parameters in `[config-file]`:
* `dataroot`: the path of your nuScenes data
* `logdir`: the path where log files, checkpoints, etc., are saved
* `batch_size`: this should be the sum of samples across all GPUs, where `sample_per_gpu` = `batch_size` / `gpu_nums`.
* `gpus`: the number of GPUs you are using.

### Evaluation

#### mIoU Metric
To evaluate your model using the mIoU metric, you should first set the `modelf` in `[config-file]` to the path of your checkpoint, and then use the following command:
```
python tools/eval.py [config-file]
```

#### mAP Metric

Before running the evaluation code, you should first obtain the `submission.json` file, which can be generated using the following command:
```
python tools/export_json.py
```
> Note: remember to set the value of `result_path` in `[config-file]`.

Run `python tools/evaluate_json.py` for evaluation.
```
python tools/evaluate_json.py
```
