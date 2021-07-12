### Tensorflow 2 Installation windows10 with CUDA and cudnn

---

1. **Install anaconda : https://www.anaconda.com/products/individual**

2. **Install visual C++ :** https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqa0ROWmhCYnY5NnJPazA3OW1yZTh3Z05GNzhTZ3xBQ3Jtc0trc3hmWlhFMGdEMU91RllNMXoxd0ZPSE9MbC1PMnVEM1A1RzAzS3NtckhoTU5vU3doTC1IcTMzOG5nNU5TQmdKVUZDc1NaMF9wajhicFJpWW8tLWVzN2lkczl3eXV0QVhGVnQtSng3QmVlbHU5RzJQRQ&q=https%3A%2F%2Fsupport.microsoft.com%2Fen-us%2Ftopic%2Fthe-latest-supported-visual-c-downloads-2647da03-1eea-4433-9aff-95f26a218cc0

3. **Check the Link https://www.tensorflow.org/install/source_windows for cuda version**

   ### GPU

   | Version              | Python version | Compiler  | Build tools | cuDNN | CUDA |
   | :------------------- | :------------- | :-------- | :---------- | :---- | :--- |
   | tensorflow_gpu-2.5.0 | 3.6-3.9        | MSVC 2019 | Bazel 3.7.2 | 8.1   | 11.2 |



4. **Create the new environment in Conda**

###### Commands :
1. conda create -n tf_gpu python==3.8

2. conda activate tf_gpu

3. conda install cudatoolkit=11.2 cudnn=8.1 -c=conda-forge

4. pip install --upgrade tensorflow-gpu

   

5. **Testing GPU is available or Not.**

```python
import tensorflow as tf
tf.test.is_gpu_available()
```

