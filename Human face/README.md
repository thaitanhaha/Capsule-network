# CNN and Capsule with human face

I constructed a dataset of human faces with their eyes and mouth swapped in position. 
Then, I performed the task of classifying the normal human faces and the edited human faces.

## First experiment

I trained both CNN and Capsule with Human Face dataset labeled as 1 and Flower dataset labeled as 0.
Then I tested with Human Face Swapped dataset.

| Model     | Accuracy |
|-----------|----------|
| CNN       |     0.0859     |
| Capsule   |     0.3984     |

## Second experiment

I train both CNN and Capsule with Human Face dataset labeled as 1 and Human Face Swapped dataset labeled as 0.
Then I tested with Human Face Swapped dataset.

| Model     | Accuracy |
|-----------|----------|
| CNN       |     0.0000     |
| Capsule   |     0.4609     |

## Conclusion

Both experiment results illustrate that the CNN cannot distinguish between the human face and the edited human face; it treats them the same, which is a disadvantage of the pooling layer. 
On the other hand, Capsule networks, without a pooling layer, treat them differently, but still do not perform well (maybe I need to adjust the layers).

