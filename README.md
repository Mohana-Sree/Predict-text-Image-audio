# Predict-text-Image-audio

A multimodal machine learning project that performs predictions based on **text**, **image**, and **audio** inputs, leveraging both **Python (FastAPI)** and **Java (Maven)** technologies.

---

## Project Structure

```
Predict-text-Image-audio/
├── FastApi/       # FastAPI backend for ML model serving
├── Maven/         # Java components, likely for audio preprocessing or backend services
└── README.md      # Project documentation
```

---

## Features

* **Text Classification** using FastAPI and NLP models.
* **Image Recognition** powered by pre-trained computer vision models.
* **Audio Analysis** possibly using signal processing or ML models for classification.
* RESTful **API endpoints** for each input type.
* Hybrid tech stack with Python and Java for modular functionality.

---

## Getting Started

### Python Setup (FastAPI)

1. Navigate to the FastAPI directory:

   ```bash
   cd FastApi
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the FastAPI server:

   ```bash
   uvicorn main:app --reload
   ```

4. Open your browser at: [http://localhost:8000/docs](http://localhost:8000/docs)

---

### Java Setup (Maven)

1. Navigate to the Maven project:

   ```bash
   cd Maven
   ```

2. Build the project using Maven:

   ```bash
   mvn clean install
   ```

> You must have Java (JDK 8+) and Maven installed.

---

## API Endpoints (Example)

### `/predict/text`

**Input:** JSON with a `text` field
**Output:** Predicted label or sentiment

### `/predict/image`

**Input:** Image file via `multipart/form-data`
**Output:** Detected object/classification

### `/predict/audio`

**Input:** Audio file (WAV/MP3)
**Output:** Audio classification result

---

## Example Request

```bash
curl -X POST "http://localhost:8000/predict/text" \
  -H "Content-Type: application/json" \
  -d '{"text": "Example input string"}'
```

---

## Technologies Used

* **FastAPI** – API backend for ML endpoints
* **TensorFlow / PyTorch** – Deep learning models (assumed)
* **OpenCV / PIL** – Image preprocessing (assumed)
* **Librosa / Pydub** – Audio processing (assumed)
* **Maven** – Java project build tool

---

## Author

Developed by [Mohana Sree](https://github.com/Mohana-Sree)
