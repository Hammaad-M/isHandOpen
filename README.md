# Usage
`isHandOpen(prediction.annotations, HAND_OPEN_BUFFER)`
- The predictions object is an element of the returned array from the Tensorflow.js HandPose model's `estimateHands` function. 
- The `HAND_OPEN_BUFFER` controls how many times in a row the hand should be detected as open before the isHandOpen function returns `true`. By default, `HAND_OPEN_BUFFER` is `null` meaning the function returns exactly what it predicts, every time.

`isHandOpen` returns `true` or `false` based on if the given information represents a closed or open hand. `true` equates to the given hand being open.

#### Usage examples can be found in the [code write-up for Touchless Interface](https://pub.towardsai.net/creating-a-touchless-interface-with-tensorflow-js-c3676582c1df "ss Interface") and the [Touchless Interface repository](https://github.com/Hammaad-M/touchless-interface "ouchless Interface Repository"). 
