# basketballVideoAnalysis

See wiki page for [more details](https://github.com/stephanj/basketballVideoAnalysis/wiki).

## mask-rcnn 

First get the frozen inference graph from link below and place this in mask-rcnn/mask-rcnn-coco directory

https://basketball-ml.s3-eu-west-1.amazonaws.com/frozen_inference_graph.pb

Now you can run the Mask RCNN application using following command

```
python mask_rcnn.py -i images/basketball.jpg -m mask-rcnn-coco -v 1
```

The masked image result is placed in the output directory including the segmented image files.

## color-detection

Run the script run.sh to execute color detection on the 25 extracted segments from the Mask R-CNN application.
The resulting colorbar images are stored in the samples directory.
