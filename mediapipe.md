## MediaPipe

[CodePen Home MediaPipe Image Segmentation Task for web](https://codepen.io/mediapipe-preview/pen/xxJNjbN) [codepen](https://codepen.io/JacobHsu/pen/mdvNMjy?editors=1010)


doc [Image embedding guide for Web](https://developers.google.com/mediapipe/solutions/vision/image_embedder/web_js)
```js
const vision = await FilesetResolver.forVisionTasks(
  // path/to/wasm/root
  "https://cdn.jsdelivr.net/npm/@mediapipe/tasks-vision@latest/wasm"
);
  const imageEmbedder = await ImageEmbedder.createFromOptions(vision, {
    baseOptions: {
      modelAssetPath: `https://storage.googleapis.com/mediapipe-models/image_embedder/mobilenet_v3_small/float32/1/mobilenet_v3_small.tflite`
    },
  });
```
