# nocaps
# nocaps: novel object captioning at scale

## About the first week of April 2019, the dataset will be released
## Introduction

‘nocaps’, for novel object captioning at scale,
the benchmark consists of 166,100 human-generated captions describing 15,100 images from the Open Images validation and test sets. 

Image captioning, the task of generating natural language descriptions of visual content, has seen rapid
progress over the past several years. However, despite continual modeling improvements and everincreasing benchmark performance, existing captioning models generalize poorly to images `in the wild`. Here `in the wild` means images outside the classes in training set.

For example, models trained on COCO captions can
typically describe images containing dogs, people and umbrellas, but not accordions or dolphins. This limits the usefulness of these models in real-world applications, such as
providing assistance for people with impaired vision, or for
improving natural language query-based image retrieval.

=> **should be able to learn from alternative data
sources – such as object detection datasets – in order to describe objects not present in the caption corpora they are
trained with**.

**_Such objects are referred to as novel objects
and the task of describing images containing novel objects
is termed novel object captioning_**

To generalize better `in the wild`, we argue that captioning models should be able to learn from alternative data
sources – such as object detection datasets – in order to describe objects not present in the caption corpora they are
trained with. Such objects are referred to as `novel objects`
and the task of describing images containing novel objects
is termed `novel object captioning`.

## Dataset

The nocaps benchmark consists of a validation set and a test set comprised of 4,500 and 10,600 images,
respectively, sourced from the Open Images object detection dataset and annotated with 11 human-generated
captions per image (comprising 10 reference captions for
automatic evaluation plus a human baseline).

- Download and extract `caption_datasets.zip` to the same directory and rename to `caption data` directory
[Andrej Karpathy's training, validation, and test splits](http://cs.stanford.edu/people/karpathy/deepimagesent/caption_datasets.zip).
- Download and extract val2014 and train2014 to `caption data/`
[Training (13GB)](http://images.cocodataset.org/zips/train2014.zip) and [Validation (6GB)]

- [Open Images V4 dataset](https://storage.googleapis.com/openimages/web/index.html)

## Evaluation
Authors report automatic evaluation metrics for the entire dataset, as well as
*in-domain*, **near-domain** and ***out-of-domain subsets*** of images containing *only COCO* classes, **both COCO and Open
Images** classes, and only ***Open Images*** classes, respectively.

