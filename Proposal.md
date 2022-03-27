Project 1 - Proposal
Using Facebook Photos API and Google App Engine to create a Social Media Application

Group 5
Akash Mahesh Mhatre - ld2746
Sanchit Thakur - ii2682
Vishnu Priya Alluri - cq5226
Lepakshi Pavani Vemula -fj4342


Using Facebook Photos API and Google Cloud Storage and Computer Vision API's to detect objects in an image and creating clusters of objects for classification of images.

Introduction:
The application will retrieve a Facebook photo from the user’s Facebook profile using Graph API and use the retrieved photo for processing results through Google SaaS Computer Vision API .
The result then will be used for Google Analytics Platform (App Engine Server Side Analytics) as it provides computing resources to collect, store, process, and report on these user-interactions to detect objects and start creating clusters of the object based on the similarity of the object to the reference object for image classification.

Proposal:
The application will be able to access the photos of users on his/her Facebook profile using the Facebook Graph API which is the primary way for the application to read and write to the Facebook Social Graph then the photos will be stored in Google DataStore. The Google VisionAI will be used to extrapolate data from photos to detect the objects and will return appropriate labels with respect to the image. Image object detection information will be used to classify the image. After extrapolation we will store the extrapolated data on the Google DataStore to fetch instantaneous data when called again in future and for further data analytics and exploration.
Sequence Diagram:
![screenshot image](https://github.com/Akash274/Project_1_web_systems/blob/main/diagrams/sequence_diagram_project_1.PNG)
Flow Chart Diagram:
![screenshot image](https://github.com/Akash274/Project_1_web_systems/blob/main/diagrams/flow_diagram_project_1.PNG)

Implementation:
The Application will be using Facebook Graph API to fetch data from the Facebook platform to access data of the user.
Facebook Graph API is the primary way to get data into and out of the Facebook platform. It's an HTTP-based API that apps can use to programmatically query data, post new stories, manage ads, upload photos, and perform a wide variety of other tasks.
After fetching Data from Facebook Graph API, data will be stored on Google DataStore for Google Saas’s cloud API
Google DataStore is a schemaless database, which allows you to worry less about making changes to your underlying data structure as your application evolves. Datastore provides a powerful query engine that allows you to search for data across multiple properties and sort as needed.
The data stored at Google DataStore will be used for image analytics and extrapolation with the help of Google VisionAI and to further classify image  according to the usage and preference of the user, the meta data of the images will be stored in the Google DataStore to further perform and functions or build over the application itself and for future extraction of data.
Google VisionAI is a platform that allows developers to easily integrate vision detection features within applications, including image labeling, face and landmark detection, optical character recognition (OCR), and tagging of explicit content.

