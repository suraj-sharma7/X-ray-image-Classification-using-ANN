🧠 Medical Image Classification with Explainable AI
📌 Objective
Build a deep learning model to classify medical images (e.g., Chest X-rays) into disease categories such as 'Normal' and 'Pneumonia'. Integrate a user-friendly interface using Gradio so that users can upload images and get predictions.
🛠️ Tools & Technologies Used
- Language: Python
- Libraries: PyTorch, Torchvision, Pillow, Gradio
- Interface: Gradio Web UI
- Model Architecture: ResNet18 (customized final layer for binary classification)
🗂️ Dataset
The model was trained on a Chest X-ray dataset containing images labeled as 'Normal' and 'Pneumonia'.
🔍 Model Description
A ResNet18 model was used as the base architecture with its final fully connected layer modified for two-class classification. The model was trained using PyTorch and saved as 'model.pth'.
🌐 Gradio Interface
Gradio was used to create an interface where users can upload a medical image and receive the model's prediction. The interface accepts an image, applies preprocessing, and returns a label ('Normal' or 'Pneumonia').
🔄 Workflow Steps
1. Load and preprocess the uploaded image using Torchvision transforms.
2. Pass the image through the trained ResNet18 model.
3. Return the predicted class label as output via the Gradio interface.
🚀 Future Enhancements
- Integrate Grad-CAM to visualize the image regions influencing predictions.
- Add more disease classes and use larger models like EfficientNet.
- Deploy as a web app using services like Hugging Face Spaces or Streamlit Cloud.
