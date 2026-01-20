FROM tensorflow/serving:latest
COPY ./models /models
# Expose the default TensorFlow Serving port
EXPOSE 8501
# Start TensorFlow Serving with the specified model
CMD ["tensorflow_model_server", "--rest_api_port=8501", "--model_name=digit_classifier", \
"--model_base_path=/models/digit_classifier"]