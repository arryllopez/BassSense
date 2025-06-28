# BassSense 🎣

BassSense is an AI-powered web application designed to help anglers optimize largemouth bass fishing techniques. By analyzing images of water bodies and combining them with environmental data such as temperature, weather, and cloud cover, BassSense recommends the best baits and strategies to improve fishing success.

## Features

- Upload a photo of your fishing location.
- Input water temperature manually.
- Retrieve live weather conditions using the OpenWeatherMap API.
- Receive AI-generated bait recommendations and strategies based on image and environmental analysis.

## Tech Stack

- Frontend: React
- Backend: Flask
- Machine Learning: PyTorch, TorchVision, NumPy
- Image Processing: Transfer learning using ResNet
- External APIs: OpenWeatherMap API
- Deployment: Docker, AWS EC2

## Installation

Clone the repository:

git clone https://github.com/yourusername/basssense.git
cd basssense

### Backend Setup

1. Create a Python virtual environment:

python -m venv venv
source venv/bin/activate      # On Windows, use venv\Scripts\activate

2. Install Python dependencies:

pip install -r requirements.txt

3. Set environment variables for your API keys, for example:

export OPENWEATHER_API_KEY=your_api_key_here

4. Run the Flask server:

flask run

### Frontend Setup

If you’re using Create React App:

cd frontend
npm install
npm start

## Usage

1. Launch the app in your browser.
2. Upload an image of your fishing spot.
3. Enter the water temperature.
4. Click **Get Recommendation**.
5. View bait suggestions based on the uploaded photo and live weather conditions.

## Model Training

BassSense uses a PyTorch model leveraging transfer learning with ResNet. Images are preprocessed and converted to feature embeddings, which are combined with environmental data like temperature and weather. A custom classifier predicts bait recommendations based on these combined features.

## Deployment

BassSense is containerized with Docker and can be deployed on AWS EC2 for testing and future scalability.

## Future Enhancements

- Fine-tune the ML model with more labeled fishing images and expert recommendations.
- Support storage of user-uploaded images using AWS S3.
- Add maps and geolocation support for location-based fishing suggestions.
- Enhance the frontend UI with advanced charting and analytics.

## License

MIT License

## Author

Your Name (your.email@example.com)
