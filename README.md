# ☀️ Number Detection Machine Learning Model 0️⃣1️⃣2️⃣

## 📌 Description

This project implements a real-time digit recognition system using a Convolutional Neural Network (CNN) trained on the MNIST dataset. Users can draw digits on an HTML5 canvas, and the model predicts the drawn number with high accuracy. Built with Python, TensorFlow, Flask, and integrated with a web interface, the application leverages ngrok for deployment and testing on Google Colab.

🖋️**Features:** 
Draw digits, real-time prediction, simple UI.

👩🏻‍💻**Tech Stack:** 
TensorFlow, Flask, HTML5 Canvas, ngrok.

▶️**Usage:** 
Run the Flask server in Colab, open the HTML file, and start drawing!

## Prerequisites

- **Python 3.x**
- **Google Colab Account** (for running the Flask server)
- **Ngrok Account** (for tunneling; free tier works)
- **Dependencies**: TensorFlow, Flask, Flask-CORS, Pyngrok, Pillow, NumPy

## 💻Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/digit-recognition.git
   cd digit-recognition
   ```

2. **Install Dependencies in Colab**:
   - Open the notebook in Google Colab.
   - Run the following command in a cell to install required packages:
     ```bash
     !pip install tensorflow flask flask-cors pyngrok pillow numpy
     ```

3. **Set Up Ngrok Authtoken**:
   - Sign up at [ngrok.com](https://ngrok.com) and get your authtoken from [dashboard.ngrok.com](https://dashboard.ngrok.com/get-started/your-authtoken).
   - In Colab, add the authtoken as a secret:
     - Go to the left sidebar, click the key icon, add a new secret named `NGROK_AUTH_TOKEN`, and paste your authtoken.

4. **Upload the Model**:
   - Ensure the trained model file `digit_recognition_cnn.h5` is available. Upload it to Colab using:
     ```python
     from google.colab import files
     files.upload()  # Upload digit_recognition_cnn.h5
     ```

5. **Download the HTML File**:
   - The `digit_recognition.html` file is provided in the repository. Download it after updating the ngrok URL (see Usage).

## 🪴Usage

1. **Run the Flask Server in Colab**:
   - Copy the Flask code into a Colab cell and run it. The code will start the server and provide a ngrok URL (e.g., `https://15313984e66b.ngrok-free.app`).
   - Example Flask code is available in the repository or previous messages.

2. **Update the HTML File**:
   - Open `digit_recognition.html` in a text editor.
   - Replace the `fetch` URL in the `predictDigit` function with the ngrok URL (e.g., `https://15313984e66b.ngrok-free.app/predict`).
   - Save and open the file in a web browser.

3. **Test the Application**:
   - Draw a digit on the canvas in the browser.
   - Click "Predict" to see the model's prediction.
   - Use "Clear Canvas" to start over.

# Output

![Digit Recognition Demo image 1](https://github.com/Bluepanda-Code/Number-Detection-ML-Model/blob/master/Output%20Images/output_example1.png)
![Digit Recognition Demo image 1](https://github.com/Bluepanda-Code/Number-Detection-ML-Model/blob/master/Output%20Images/output_example2.png)
![Digit Recognition Demo image 1](https://github.com/Bluepanda-Code/Number-Detection-ML-Model/blob/master/Output%20Images/output_example3.png)

## 🦾Project Structure

- `digit_recognition_cnn.h5`: The trained CNN model file.
- `digit_recognition.html`: The web interface for drawing and predicting digits.
- `README.md`: This file.

## 🆘Contributing

Contributions are welcome! Please fork the repository and submit pull requests for any improvements (e.g., UI enhancements, model optimization).

## 🪪License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧Contact

For questions or support, please open an issue on the GitHub repository or contact the maintainer at [namanvish072@gmail.com](mailto:namanvish072@gmail.com).

```
