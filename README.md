# KiranaCheckout

“When the world is moving faster than ever, why should the process of creating /updating your application environment be slow and manual?”

Edge' is a technology buzzword trending for being a frontier technology. Cloud technology and services have been extensively used by large percentage of consumers, however most of the new upcoming opportunities lie at the 'Edge'. With Edge Computing, data is not sent to the Cloud but acted on at the source, creating real-time insights. The likes of 5G, Autonomous vehicles, Smart City, etc have Edge computing as the de-facto technology. The parasol of Edge computing involves concerted use of Artificial Intelligence, Machine Learning, Internet of Things, Service Operations and Blockchain. Edge Computing drives the foundational grounds for various domain requirements and imperative elements of technology.

In Kirana Stores, the traditional system of buying items is manual and very slow indeed. In order to make it faster and more efficient. We devise a system that allows automatic detection of product using camera. For example, if a toothpaste is placed in front of the camera, it detects the product and details of each product scanned is then presented at the bill of materials for payment.

Our System is not compute intensive and the scanning is done in real time without sending the data to cloud for processing as some of these stores can be in remote areas with intermittent connectivity and we do not want the customers to wait due to latency issues for connectivity.

The application can detect, count, appropriately price oranges, apples, and bananas and finally add them to a shopping list. The idea is simple, we train a model using the TensorFlow Object Detection API and build a web application using Flask and ReactJS.

To be more specific, we trained a model and fed it with a small labelled image dataset of some items which are seen commonly seen in Kirana stores that we created then trained it. 

Secondly, we developed an inference application using Flask (backend) and ReactJS (frontend). Basically, the ReactJS app uses the system’s camera to capture an image and send it via API to the Flask backend, where the model is hosted. After the prediction is made it returns the results to the frontend, to print it on the User Interface.

These are the basic steps that were followed:
    1. Data preparation.
    2. Train a model using transfer learning.
    3. Build the app backend using Flask microframework.
    4. Build the app frontend (UI) using ReactJS.
    5. Containerize the app using Docker.
