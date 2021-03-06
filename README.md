# Revisiting Oxford and Paris: Large-Scale Image Retrieval Benchmarking

<img src="http://cmp.felk.cvut.cz/revisitop/img/revisitop_teaser_medium.png" width=\textwidth/>

## MATLAB

Tested with MATLAB R2017a on Debian 8.1.

### Process images

Example script that describes how to: read and process database images; read, crop and process query images:
```
>> example_process_images
```
It automatically downloads dataset images, and revisited annotation file.

### Evaluate results

Example script that describes how to evaluate revisited annotation and three protocol setups:
```
>> example_evaluate
```
It automatically downloads dataset images, revisited annotation file, and example features (R-[37]-GeM from the paper) to be used in the evaluation.
Final output should look like this (depending on the selected ```test_dataset```):
```
>> roxford5k: mAP E: 84.81, M: 64.67, H: 38.47
>> roxford5k: mP@k[1 5 10] E: [97.06 92.06 86.49], M: [97.14 90.67 84.67], H: [81.43 63.00 53.00]
```
or
```
>> rparis6k: mAP E: 92.12, M: 77.20, H: 56.32
>> rparis6k: mP@k[1 5 10] E: [100.00 97.14 96.14], M: [100.00 98.86 98.14], H: [94.29 90.29 89.14]
```

## Python

Tested with Python 3.5.3 on Debian 8.1.

### Process images

Example script that describes how to: read and process database images; read, crop and process query images:
```
>> python3 example_process_images
```
It automatically downloads dataset images, and revisited annotation file.

### Evaluate results

Example script that describes how to evaluate revisited annotation and three protocol setups:
```
>> python3 example_evaluate
```
It automatically downloads dataset images, revisited annotation file, and example features (R-[37]-GeM from the paper) to be used in the evaluation.
Final output should look like this (depending on the selected ```test_dataset```):
```
>> roxford5k: mAP E: 84.81, M: 64.67, H: 38.47
>> roxford5k: mP@k[ 1  5 10] E: [97.06 92.06 86.49], M: [97.14 90.67 84.67], H: [81.43 63.   53.  ]
```
or
```
>> rparis6k: mAP E: 92.12, M: 77.2, H: 56.32
>> rparis6k: mP@k[ 1  5 10] E: [100.    97.14  96.14], M: [100.    98.86  98.14], H: [94.29 90.29 89.14]
```

## Related publication

```
@inproceedings{Radenovic-CVPR18,
 author = {Radenovi\'{c}, F. and Iscen, A. and Tolias, G. and Avrithis, Y. and Chum, O.},
 title = {Revisiting Oxford and Paris: Large-Scale Image Retrieval Benchmarking},
 booktitle={CVPR},
 year={2018}
}
```