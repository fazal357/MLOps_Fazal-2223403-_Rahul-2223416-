# Flask Image Classifier ML Model Demo with Docker

This project demonstrates how to deploy a machine learning image classifier model using Flask and containerize the service with Docker. Users can upload images via a simple web interface and get predictions from a pre-trained ResNet50 model.

## Features
- Flask-based web app with HTML templates for file upload
- Uses Keras ResNet50 model for image classification
- Dockerized for easy deployment and environment consistency
- Bootstrap for basic styling

## Project Structure
├── app.py # Flask application code
├── requirements.txt # Python dependencies
├── Dockerfile # Docker image build instructions
├── templates/
│ └── index.html # HTML template for the app UI
├── images/ # Folder where uploaded images are saved

text

## Setup and Run Locally

1. Install dependencies:

pip install -r requirements.txt

text

2. Run the Flask app:

python app.py

text

3. Open your browser to [http://localhost:3000](http://localhost:3000)

## Docker Build and Run

1. Build the Docker image:

docker build -t flask-ml-demo .

text

2. Run the container:

docker run -p 3000:3000 flask-ml-demo

text

3. Access the app at [http://localhost:3000](http://localhost:3000)

## Usage

- Upload any image via the input form
- Click "Predict Image" button
- View the prediction label displayed on the page

## Notes

- Uploaded images are saved in the `images/` directory inside the container
- The model used is Keras' pre-trained ResNet50
- This is a demo project for educational purposes and not optimized for production

## Dependencies

See `requirements.txt` for Python package details including Flask, Keras, TensorFlow, and Bootstrap (via CDN).

## License

MIT License

---
