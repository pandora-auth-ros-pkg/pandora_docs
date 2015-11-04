# Headers


Every header file should have the appropriate header guards


Suppose the following directory tree:

```
|-- pandora_vision_victim/
|   |-- include/
|   |   |-- pandora_vision_victim/
|   |   |   |-- classifiers
|   |   |   |   |-- abstract_classifier.h
```

Inside `abstract_classifier.h` we add the following:

```cpp
#ifndef PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H
#define PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H

/**
 * Code here
 */

#endif  // PANDORA_VISION_VICTIM_CLASSIFIERS_ABSTRACT_CLASSIFIER_H
```

The name of the header guard derives from the name of the package and the
following subdirectories and the file name written in [SNAKE_CASE](https://en.wikipedia.org/wiki/Snake_case).

