# Prodigy_infotech_Ml_Task5
PRODIGY_INFOTECH_TASK5_FOOD_PREDICTION
🍽️ PRODIGY_ML_TASK_05 — Food Recognition & calories ML internship....

📌 Task Description

Develop a model that can accurately recognize food items from images and estimate their calorie content, enabling users to track their dietary intake and make informed food choices.

This project is part of the Prodigy InfoTech Machine Learning Internship — Task 05.

🔗 Repository Link https://github.com/ganeshmpsmg/Prodigy_infotech_Ml_Task5

📊 Dataset Property Details Dataset Food-11 Image Data set Source Kaggle — trolukovich/food11-image-dataset ,Total Images~16,643 SplitsTraining / Validation / Evaluation 🍱 Food Categories: Bread · Dairy Product · Dessert · Egg · Fried Food · Meat · Noodles-Pasta · Rice · Seafood · Soup · Vegetable-Fruit

🧠 Model Architecture

Base Model: MobileNetV2 (pretrained on ImageNet) Transfer Learning: Frozen base layers + custom classification head Custom Layers:

GlobalAveragePooling2D Dense(128, activation='relu') Dropout(0.3) Dense(11, activation='softmax')

🔥 Calorie Map (per 100g) Food ItemCalories (kcal)Bread265Dairy Product150Dessert350Egg155Fried Food400Meat250Noodles-Pasta220Rice206Seafood150Soup80Vegetable-Fruit60

⚙️ Installation & Setup

Clone the Repository bashgit clone https://github.com/ganesmpsmg/PRODIGY_INFOTECH_TASK5_FOOD_PREDICTION.git cd PRODIGY_INFOTECH_TASK5_FOOD_PREDICTION
Install Dependencies bashpip install -r requirements.txt
Set Up Kaggle API
Go to Kaggle Account → Create API Token Place kaggle.json at: 🚀 How to Run Step 1 — Download & Load Dataset pythonimport kagglehub path = kagglehub.dataset_download("trolukovich/food11-image-dataset") Step 2 — Build & Train Model pythonhistory = model.fit( train_data, epochs=10, validation_data=val_data, callbacks=callbacks ) Step 3 — Predict & Estimate Calories pythonestimate_calories("your_food_image.jpg")

📈 Results

📈 Results
Metric	Value
Training Accuracy	91.38%
Validation Accuracy	82.71%
Training Loss	0.2586
Validation Loss	0.5752
Prediction Confidence	99.96%
Training Time	253s (819ms/step)
Optimizer	Adam
Epochs	10
Batch Size	32
Image Size	224 x 224
🛠️ Tech Stack ToolPurposePython 3.8+Core LanguageTensorFlow / KerasDeep Learning FrameworkMobileNetV2Pretrained Base ModelKaggleHubDataset DownloadNumPy / PandasData ProcessingMatplotlibVisualizationOpenCV / PillowImage Processing

👨‍💻 Author Ganesh MP

GitHub: https://github.com/ganeshmpsmg/Prodigy_infotech_Ml_Task5

🏢 Internship Details DetailInfoOrganizationProdigy InfoTechDomainMachine LearningTaskTask 05 — Food Recognition & Calorie EstimationRepo NamePRODIGY_ML_TASK_05

📄 License This project is licensed under the MIT License — see the LICENSE file for details.

Made with ❤️ during Prodigy InfoTech ML Internship

I have successfully completed ML Internship Task 5. In the task description, the Food-101 dataset was suggested for the project. However, due to storage limitations on my laptop (since Food101 requires several GB of space), I used the Food-11 dataset instead.

Food11 is also a food image classification dataset and is similar in nature to Food101, so the same machine learning concepts and workflow could be applied effectively.

Thank you.
