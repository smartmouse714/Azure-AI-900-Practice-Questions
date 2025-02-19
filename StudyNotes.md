# What is AI?

AI is the creation of software that imitates human behaviors and capabilities. Key workloads include:

- Machine learning
: This is often the foundation for an AI system, and is the way we "teach" a computer model to make predictions and draw conclusions from data.
- Anomaly detection
: The capability to automatically detect errors or unusual activity in a system.
In Azure, the Anomaly Detector service provides an application programming interface (API) that developers can use to create anomaly detection solutions.
- Computer vision
: The capability of software to interpret the world visually through cameras, video, and images.
- Natural language processing
: The capability for a computer to interpret written or spoken language, and respond in kind.
- Knowledge mining
: The capability to extract information from large volumes of often unstructured data to create a searchable knowledge store. 

# What are AI services?

|Service|Description|
|-|-|
|Anomaly Detector|Identify potential problems early on|
|Azure Cognitive Search|Bring AI-powered cloud search to your mobile and web apps|
|Azure OpenAI|Perform a wide variety of natural language tasks|
|Bot Service|Create bots and connect them across channels|
|Content Moderator (retired)|Detect potentially offensive or unwanted content|
|Content Safety|An AI service that detects unwanted contents|
|Custom Vision|Customize image recognition to fit your business|
|Document Intelligence|Turn documents into usable data at a fraction of the time and cost|
|Face|Detect and identify people and emotions in images|
|Immersive Reader|Help users read and comprehend text|
|Language|Build apps with industry-leading natural language understanding capabilities|
|Language understanding (retired)|Understand natural language in your apps|
|Metrics Advisor|An AI service that detects unwanted contents|
|Personalizer|Create rich, personalized experiences for each user|
|QnA maker (retired)|Distill information into easy-to-navigate questions and answers|
|Speech|Speech to text, text to speech, translation and speaker recognition|
|Translator|Translate more than 100 languages and dialects|
|Video Indexer|Extract actionable insights from your videos|
|Vision|Analyze content in images and videos|

---
## Computer vision capabilities
- Image classification 
: Image classification involves training a machine learning model to classify images based on their contents. For example, in a traffic monitoring solution you might use an image classification model to classify images based on the type of vehicle they contain, such as taxis, buses, cyclists, and so on.
- Object detection 
: Object detection machine learning models are trained to classify individual objects within an image, and identify their location with a bounding box. For example, a traffic monitoring solution might use object detection to identify the location of different classes of vehicle.
- Semantic segmentation 
: Semantic segmentation is an advanced machine learning technique in which individual pixels in the image are classified according to the object to which they belong. For example, a traffic monitoring solution might overlay traffic images with "mask" layers to highlight different vehicles using specific colors.
- Image analysis
: You can create solutions that combine machine learning models with advanced image analysis techniques to extract information from images, including "tags" that could help catalog the image or even descriptive captions that summarize the scene shown in the image.
- Face detection, analysis, and recognition
: Face detection is a specialized form of object detection that locates human faces in an image. This can be combined with classification and facial geometry analysis techniques to recognize individuals based on their facial features.
- OCR
: Optical chaacter recognition is a technique used to detect and read text in images. You can use OCR to read text in photographs (for example, road signs or store fronts) or to extract information from scanned documents such as letters, invoices, or forms.

|Service|Capabilities|
|-|-|
|Azure AI Vision|You can use this service to analyze images and video, and extract descriptions, tags, objects, and text.|
|Azure AI Custom Vision|Use this service to train custom image classification and object detection models using your own images.|
|Azure AI Face|The Azure AI Face service enables you to build face detection and facial recognition solutions.|
|Azure AI Document Intelligence|Use this service to extract information from scanned forms and documents.|

---
## NLP
NLP enables you to create software that can:
- Analyze and interpret text in documents, email messages, and other sources.
- Interpret spoken language, and synthesize speech responses.
- Automatically translate spoken or written phrases between languages.
- Interpret commands and determine appropriate actions.

|Service|Capabilities|
|-|-|
|Azure AI Language|Use this service to access features for understanding and analyzing text, training language models that can understand spoken or text-based commands, and building intelligent applications.|
|Azure AI Translator|Use this service to translate text between more than 60 languages.|
|Azure AI Speech|Use this service to recognize and synthesize speech, and to translate spoken languages.|
|Azure AI Bot Service|This service provides a platform for conversational AI, the capability of a software "agent" to participate in a conversation. Developers can use the Bot Framework to create a bot and manage it with Azure Bot Service - integrating back-end services like Language, and connecting to channels for web chat, email, Microsoft Teams, and others.|

---
## Azure ML

Regression predicts a numeric *label* or outcome based on variables, or *features*.
Regression is an example of a *supervised* machine learning technique in which you train a model using data that includes both the features and known values for the label, so that the model learns to *fit* the feature combinations to the label. Then, after training has been completed, you can use the trained model to predict labels for new items for which the label is unknown.

To use Azure Machine Learning, you first create a *workspace* resource in your Azure subscription.
A workspace must be created before you can access Machine Learning studio. 
A dataset is required to create an automated machine learning (automated ML) run.
A job must be created in Machine Learning studio to use Machine Learning to train a regression model.

A dataset is required to create an automated machine learning (automated ML) run. A workspace must be created before you can access Machine Learning studio. An Azure container instance and an AKS cluster can be created as a deployment target, after training of a model is complete.

To deploy a predictive service from a newly trained model by using the Machine Learning designer, you must first create a pipeline in the Machine Learning designer. Adding training modules by using the Machine Learning designer takes place before creating a trained model, which already exists. Adding a dataset by using the Machine Learning designer requires that a pipeline already exists. To create an inferencing cluster, you must use Machine Learning studio.

### Azure Machine Learning compute
- Compute Instances
: Development workstations that data scientists can use to work with data and models.
- Compute Clusters
: Scalable clusters of virtual machines for on-demand processing of experiment code.
- Inference Clusters
: Deployment targets for predictive services that use your trained models.
- Attached Compute
: Links to existing Azure compute resources, such as Virtual Machines or Azure Databricks clusters.

1. Prepare data
: Identify the features and label in a dataset. Pre-process, or clean and transform, the data as needed.
2. Train model
: Split the data into two groups, a training and a validation set. Train a machine learning model using the training data set. Test the machine learning model for performance using the validation data set.
3. Evaluate performance
: Compare how close the model's predictions are to the known labels.
4. Deploy a predictive service
: After you train a machine learning model, you need to convert the training pipeline into a real-time inference pipeline. Then you can deploy the model as an application on a server or device so that others can use it.

Multiple linear regression models a relationship between two or more features and a single label, which matches the scenario in this item. 
Linear regression uses a single feature. 
Logistic regression is a type of classification model, which returns either a Boolean value or a categorical decision. 
Hierarchical clustering groups data points that have similar characteristics.

|Feature|Capability|
|-|-|
|Automated machine learning|This feature enables non-experts to quickly create an effective machine learning model from data.|
|Azure Machine Learning designer|A graphical interface enabling no-code development of machine learning solutions.|
|Data and compute management|Cloud-based data storage and compute resources that professional data scientists can use to run data experiment code at scale.|
|Pipelines|Data scientists, software engineers, and IT operations professionals can define pipelines to orchestrate model training, deployment, and management tasks.|

*Classification* is a form of machine learning that is used to predict which category, or class, an item belongs to. This machine learning technique can be applied to binary and multi-class scenarios.

The confusion matrix is a tool used to assess the quality of a classification model's predictions. It compares predicted labels against actual labels.

In a binary classification model where you're predicting one of two possible values, the confusion matrix is a 2x2 grid showing the predicted and actual value counts for classes 1 and 0. It categorizes the model's results into four types of outcomes. Using our diabetes example these outcomes can look like:

- True Positive
: The model predicts the patient has diabetes, and the patient does actually have diabetes.
- False Positive
: The model predicts the patient has diabetes, but the patient doesn't actually have diabetes.
- False Negative
: The model predicts the patient doesn't have diabetes, but the patient actually does have diabetes.
- True Negative
: The model predicts the patient doesn't have diabetes, and the patient actually doesn't have diabetes.

---
## Understand Responsible AI
- Fairness
- Reliability and safety
- Privacy and security
- Inclusiveness
- Transparency
- Accountability

|Challenge or Risk|Example|
|-|-|
|Bias can affect results|A loan-approval model discriminates by gender due to bias in the data with which it was trained|
|Errors may cause harm|An autonomous vehicle experiences a system failure and causes a collision|
|Data could be exposed|A medical diagnostic bot is trained using sensitive patient data, which is stored insecurely|
|Solutions may not work for everyone|A home automation assistant provides no audio output for visually impaired users|
|Users must trust a complex system|An AI-based financial tool makes investment recommendations - what are they based on?|
|Who's liable for AI-driven decisions?|An innocent person is convicted of a crime based on evidence from facial recognition – who's responsible?|

---
### Azure Cognitive Search features:

- Data from any source
: Azure Cognitive Search accepts data from any source provided in JSON format, with auto crawling support for selected data sources in Azure.
- Full text search and analysis
: Azure Cognitive Search offers full text search capabilities supporting both simple query and full Lucene query syntax.
- AI powered search
: Azure Cognitive Search has Azure AI capabilities built in for image and text analysis from raw content.
- Multi-lingual
: Azure Cognitive Search offers linguistic analysis for 56 languages to intelligently handle phonetic matching or language-specific linguistics. Natural language processors available in Azure Cognitive Search are also used by Bing and Office.
- Geo-enabled
: Azure Cognitive Search supports geo-search filtering based on proximity to a physical location.
- Configurable user experience
: Azure Cognitive Search has several features to improve the user experience including autocomplete, autosuggest, pagination, and hit highlighting.