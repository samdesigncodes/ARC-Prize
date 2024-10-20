# ARC-Prize 2024 Project Summary

![image](https://github.com/user-attachments/assets/e1be4a72-4edd-4ddb-b857-ba8b61a8cd9f)
![image](https://github.com/user-attachments/assets/8374ba97-70bc-4c81-bdea-e49a3d33e700)
![image](https://github.com/user-attachments/assets/872eaa97-8eb4-4a0f-874f-8de70faf531a)


![2_00d62c1b](https://github.com/user-attachments/assets/4c7d3240-dc9e-4348-a289-db6a1d5a493a)

![IMG_20241006_232217](https://github.com/user-attachments/assets/b7b20dba-7273-4f3a-8951-376ef62bd641)

![136_5c0a986e](https://github.com/user-attachments/assets/60f220cc-3b2a-4ad8-b2ac-da6f662431e6)

![image](https://github.com/user-attachments/assets/191a15d0-cbd7-4a5c-88d2-2a6ae7850f04)


In this project, I developed an advanced solution for the Abstraction and Reasoning Challenge (ARC) using a Recurrent Neural Network (RNN) combined with a novel branched learning approach. The central concept behind this method was to generate pixel predictions sequentially, leveraging Accuracy First Search to refine these outputs iteratively. Each predicted output was fed back into the model for subsequent iterations, forming a feedback loop that improved accuracy over time by adjusting based on the evolving output. This recursive process was essential in handling the complex pixel relationships inherent in ARC tasks.

The branched learning approach distinguished itself by focusing on iterating through multiple potential outputs rather than settling on a single result early on. This methodology enabled the model to progressively refine correct pixels in each pass. One of the key advancements was in the feedback system, where the model dynamically adjusted its predictions at each step, ensuring that every iteration contributed to an increasingly refined solution. This created a system capable of overcoming traditional single-pass neural network limitations.

![image](https://github.com/user-attachments/assets/4212ea8b-b531-4fff-a1a1-6fe9fa256cb0)


A major challenge encountered was identifying the optimal number of iterations during the intermediate inference process. Initially, I relied on accuracy as an indicator to increase iterations, but this proved insufficient for all tasks. To address this, I introduced custom metrics and adaptive rules that better reflected the model's proximity to the correct solution. These enhancements allowed the system to generalize better, especially when the direct path to the solution wasn’t clear, and pixel-based milestones were insufficient.

![image](https://github.com/user-attachments/assets/df8be02f-e4e7-4a58-a710-086edcad9092)

To implement this system, I leveraged advanced machine learning frameworks. PyTorch and PyTorch Lightning were used for designing the neural network architecture, with Hydra employed for dynamic configuration management, making it easier to experiment with various model parameters. Visualization tools, such as Rich, played a crucial role in monitoring and formatting outputs, allowing for real-time debugging and performance tracking. This combination of tools not only optimized model performance but also streamlined the development process by providing flexibility in experimentation.

The iterative development process saw significant improvements in both model accuracy and generalization. Early models struggled with tasks requiring complex pixel relationships, but by refining the recursion and incorporating more adaptive learning mechanisms, the model became more capable of handling abstract reasoning tasks. The project's current version represents a sophisticated model that intelligently balances recursion and performance metrics to achieve high accuracy in various ARC tasks.

In conclusion, the solution represents a highly advanced and optimized neural network system tailored for solving ARC tasks. By incorporating a combination of RNNs, branched learning, and iterative refinement, the model is able to handle tasks with complex pixel dependencies and adapt dynamically through recursion. The integration of advanced tools and adaptive metrics further enhances its ability to generalize across different tasks, making it a robust solution for the ARC challenge.

![image](https://github.com/user-attachments/assets/4b46e35a-9e41-45fa-8036-1a2728a5893e)

![image](https://github.com/user-attachments/assets/7dddd8d6-438f-4e8b-a9c6-c9333a570d4c)


## Popular Tools and Frameworks Used in the Model
In this project, several powerful tools and frameworks were utilized to create an advanced neural network solution for ARC:
1.	PyTorch & PyTorch Lightning: These were the core libraries for developing, training, and managing the RNN model. PyTorch provided flexibility in defining complex neural architectures, while PyTorch Lightning enabled clean, scalable experimentation.
2.	Hydra: Hydra streamlined configuration management, allowing the dynamic adjustment of hyperparameters, training configurations, and iterations.
3.	TensorFlow/Keras: For users building neural networks like RNNs or CNNs, TensorFlow provides a powerful backend, and Keras adds a simplified API for rapid development. Both tools are widely popular for RNN applications.
4.	Rich: This tool was essential for enhanced visualization and output formatting during the model's execution, helping track performance and debug effectively in real-time.
5.	Visual Studio Code (VS Code): The development environment for this project was primarily in VS Code, a highly customizable and feature-rich IDE, offering integrations with version control, debugging, and Python tools for seamless development.
6.	Jupyter Notebooks: These are highly interactive notebooks that simplify the coding, testing, and visualization process, often integrated into both VS Code and Google Colab for an interactive, real-time coding experience.
7.	Google Colab with GPU Support: Google Colab provided an interactive environment for testing and scaling the model, offering GPU and TPU support to accelerate the training and inference processes. This enabled faster experimentation on large datasets and deep neural networks.
8.	Jupyter Notebooks: These are highly interactive notebooks that simplify the coding, testing, and visualization process, often integrated into both VS Code and Google Colab for an interactive, real-time coding experience.




