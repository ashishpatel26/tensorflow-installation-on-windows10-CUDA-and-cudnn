### Tensorflow 2 Installation On Windows10 with CUDA and cudnn

![image-20210712165459686](https://raw.githubusercontent.com/ashishpatel26/tensorflow-installation-on-windows10-CUDA-and-cudnn/main/images/image-20210712165459686.png)

---

1. **Install anaconda : https://www.anaconda.com/products/individual**

   ![](https://raw.githubusercontent.com/ashishpatel26/tensorflow-installation-on-windows10-CUDA-and-cudnn/main/images/anaconda.png)

2. **Install visual C++ :** https://support.microsoft.com/en-us/topic/the-latest-supported-visual-c-downloads-2647da03-1eea-4433-9aff-95f26a218cc0

   ![](https://raw.githubusercontent.com/ashishpatel26/tensorflow-installation-on-windows10-CUDA-and-cudnn/main/images/c%2B%2B.png)

3. **Check the Link https://www.tensorflow.org/install/source_windows for cuda version**

   ![](https://raw.githubusercontent.com/ashishpatel26/tensorflow-installation-on-windows10-CUDA-and-cudnn/main/images/TensorflowCuda.png)

   ### GPU

   | Version              | Python version | Compiler  | Build tools | cuDNN | CUDA |
   | :------------------- | :------------- | :-------- | :---------- | :---- | :--- |
   | tensorflow_gpu-2.5.0 | 3.6-3.9        | MSVC 2019 | Bazel 3.7.2 | 8.1   | 11.2 |

4. **Create the new environment in Conda**

###### Commands :
1. ```bash
   conda create -n tf_gpu python==3.8
   ```
2. ```bash
   conda activate tf_gpu
   ```

3. ```bash 
   conda install cudatoolkit=11.2 cudnn=8.1 -c=conda-forge
   ```

4.  ```bash
    pip install --upgrade tensorflow-gpu
    ```


5. **Testing GPU is available or Not.**

```python
import tensorflow as tf
tf.test.is_gpu_available()
```

6. **Installation of CUDA Toolkit as well** - **[Download CudaToolkit](https://developer.nvidia.com/cuda-downloads)**

   ![](https://cdn.ourcodeworld.com/public-media/gallery/gallery-5ff6217950d99.png)

   **Thanks for Reading**

   ---

   
