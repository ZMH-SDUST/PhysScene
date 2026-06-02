# Experiment Settings

## Hyperparameter Configuration

For all experiments, we used the default parameter settings provided by the official implementations of the corresponding baseline models. No special hyperparameter tuning was conducted.

For detailed model configurations, please refer to the related code repositories and paper links provided in this project.

## Experimental Hardware

All experiments were conducted on the following hardware:

- 4 NVIDIA RTX 3090 GPUs

## Data Splitting Strategy

We used `random.shuffle` to randomly shuffle the data before splitting. The random seed was fixed as:

```text
Seed = 1234
```

## CS-SGG Setting

For the **CS-SGG** setting, we performed a sample-level random split.

## OvD-SGG Setting

For the **OvD-SGG** setting, we performed a random split based on the object type list.

The complete object list is:

```text
[
  "Electronic Balance",
  "Disk",
  "Weight Box",
  "Hand",
  "Vernier Caliper",
  "Glass Dish",
  "Regular Object",
  "Base Screw",
  "Hanging Ring",
  "Optical Axis",
  "Lifting Screw",
  "Triangular Level",
  "Paper",
  "Objective Focusing Knob",
  "Weight V2",
  "Specimen Stage V2",
  "Beaker",
  "Ring",
  "Zero Adjustment Knob",
  "Irregular Object",
  "Circular Pulley",
  "Stand Screw",
  "Person",
  "Fixed Stage V1",
  "Tweezers",
  "Weight Prism",
  "Rotational Inertia Apparatus",
  "Eyepiece Focusing Knob V1",
  "Vernier Dial",
  "Base Screw V1"
]
```

## OvR-SGG Setting

For the **OvR-SGG** setting, we performed a random split based on the relation type list.

The complete relation list is:

```text
[
  "Reflective",
  "Measure",
  "Fold",
  "Plastic",
  "Touch",
  "Record",
  "Inside",
  "Rotate V1",
  "Blurry",
  "Lift",
  "Glass",
  "Fix",
  "Near",
  "Observe",
  "Suspend",
  "Metallic",
  "Tap",
  "Mixed Color",
  "Drag",
  "Clip",
  "White",
  "Press",
  "Transparent",
  "Pull Out",
  "Grab",
  "Black",
  "Part Of",
  "Move",
  "Rotate V2",
  "Read",
  "Adjust",
  "Hold",
  "Push-Pull",
  "Unpack",
  "Knock",
  "In Front Of",
  "Frosted",
  "Pinch"
]
```
