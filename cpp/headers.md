# Headers


1. Every header file should have the appropriate header guards


Suppose the following directory tree:

```
|-- pandora_vision_victim/
|   |-- include/
|   |   |-- pandora_vision_victim/
|   |   |   |-- classifiers
|   |   |   |   |-- abstract_classifier.h
```

```cpp
#ifndef PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H
#define PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H

/**
 * Code here
 */

#endif  // PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H
```
