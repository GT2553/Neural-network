# Neural-Networks--2

Student Name: Gnanadeep Tadikonda \
ID: 700759736
gmail:gxt97360@ucmo.edu

Question 1: Cloud Computing for Deep Learning 
(a) Elasticity and Scalability in Cloud Computing for Deep Learning (10 points)
Elasticity:

The ability of a cloud system to dynamically allocate and deallocate resources based on workload demands.
Ensures cost-efficiency by scaling resources up during high demand and down during low demand.
Example: Automatically provisioning more GPUs when training large deep learning models and reducing them after completion.
Scalability:

The ability of a cloud system to handle increasing workloads by adding more resources (scaling up or out).
Two types:
Vertical Scaling (Scale-Up): Increasing compute power (CPU, GPU, RAM) of a single instance.
Horizontal Scaling (Scale-Out): Adding more instances/nodes to distribute workloads.
Example: Expanding a distributed training system across multiple GPUs or cloud instances.

(b) Comparison of AWS SageMaker, Google Vertex AI, and Azure ML Studio (10 points)
1. AWS SageMaker
✅ Fully managed ML service with integrated Jupyter notebooks.
✅ Supports TensorFlow, PyTorch, MXNet, and Scikit-learn.
✅ Auto-scaling for distributed training and model deployment.
✅ Supports Nvidia GPUs and AWS Inferentia for optimized deep learning.
✅ Offers MLOps tools like Pipelines, AutoML, and model monitoring.
✅ Best for enterprise-level scalable AI workloads.

2. Google Vertex AI
✅ Unified platform integrating AutoML and custom ML models.
✅ Supports TensorFlow, PyTorch, and Scikit-learn.
✅ Kubernetes-based distributed training for scalability.
✅ Supports GPUs and TPUs for accelerated AI workloads.
✅ Includes Vertex Pipelines, AI Explanations, and AutoML.
✅ Best for data-centric AI with strong AutoML capabilities.

3. Microsoft Azure Machine Learning Studio
. Low-code/no-code interface for ML model development.
. Supports TensorFlow, PyTorch, ONNX, and Scikit-learn.
 .Offers hyperparameter tuning and distributed training.
.Supports Nvidia GPUs and FPGAs for deep learning.
. Provides MLOps, CI/CD integration, and AutoML.
. Best for users within the Microsoft ecosystem (Azure, Power BI, Synapse).

Question 3: CNN Feature Extraction with Filters and Pooling (30 points)
Task 1: Implement Edge Detection Using Convolution (15 points)
Explanation:
•	Loads a grayscale image. \
•	Defines the Sobel filters for detecting edges in the x and y directions. \
•	Applies convolution using cv2.filter2D(). \
Displays the original and filtered images using matplotlib \

Task 2: Implement Max Pooling and Average Pooling (15 points)
Explanation: \
1.	Generates a random 4×4 matrix with values between 0 and 9. \
2.	Uses MaxPooling2D for max pooling and AveragePooling2D for average pooling. \
3.	Strides = 2, Pool size = 2×2, meaning the pooled output will be 2×2. \
4.	Prints the original, max-pooled, and average-pooled matrices. \

Question 4: Implementing and Comparing CNN Architectures (30 points)
Task 1: Implement AlexNet Architecture (15 points)
Explanation:
1.	First Convolutional Layer:
o	96 filters, (11×11) kernel, stride 4, ReLU activation
o	Followed by MaxPooling (3×3) with stride 2
2.	Second Convolutional Layer:
o	256 filters, (5×5) kernel, ReLU activation
o	MaxPooling (3×3) with stride 2
3.	Third, Fourth, and Fifth Convolutional Layers:
o	384, 384, and 256 filters with (3×3) kernel, ReLU activation
o	MaxPooling (3×3) with stride 2 after the fifth layer
4.	Flatten layer to convert feature maps to a 1D vector
5.	Two Fully Connected (Dense) Layers:
o	4096 neurons each, ReLU activation, Dropout (50%)
6.	Output Layer:
o	10 neurons, softmax activation for classification
Output:
After running the script, you’ll see the model summary showing layer details, output shapes, and parameter counts.

Task 2: Implement a Residual Block and ResNet (15 points)
Step 1: Implement Residual Block
•	Takes an input tensor.
•	Applies two Conv2D layers (each with 64 filters, (3×3) kernel, ReLU activation).
•	Includes a skip connection (adds input to output before activation).
🔹 Step 2: Build a Simple ResNet-like Model
•	Initial Conv2D layer (64 filters, (7×7) kernel, stride 2).
•	Apply two residual blocks.
•	End with a Flatten layer, Dense layer (128 neurons), and Output layer (Softmax)
Output: The script will print the model summary for the ResNet-like model, showing:
•	Layers: Conv2D, Residual Blocks, Flatten, Dense.
•	Parameters for each layer.




