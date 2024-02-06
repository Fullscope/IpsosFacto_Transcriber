# Use the official Python 3.10.13 image as the base image
FROM python:3.10.13

# Install necessary dependencies including git, ffmpeg, and rust

RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
    software-properties-common \
    git \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory to /app
WORKDIR /app

# Clone the private GitHub repository
RUN git clone https://github.com/Fullscope/IpsosFacto_Transcriber.git


# Install the required Python packages
RUN pip install -r requirements.txt

# Expose the default Streamlit port
EXPOSE 8501

# Set the entrypoint command to run the Streamlit app
CMD ["streamlit", "run", "app.py"]
