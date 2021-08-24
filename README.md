# Car Crossing Detection

This is my graduate work for the Specialization in AI at the Escola Politécnica da USP (Poli-USP).

This work consists in a detection algorithm for vehicle street corner crossings using camera data.

This work will be made using Python 3.7, due to usage of several tools (such as dataclasses) and the libraries OpenCV, numpy, tensorflow and poetry (package management). For the deployment, Docker container will be used in the GCP Docker registry and will be acessible by a Flask application.

The model will detect 3 classes:
- Bikes
- Buses
- Cars

# Data

The data for this project was donated by the CET (Central de Engenharia de Tráfego), which is the company responsible for traffic management in the city of São Paulo.

There's also a [live feed](http://cameras.cetsp.com.br/View/Cam.aspx) for the CET cameras and it may be used for gathering more data.

## Preprocessing

The images are in video format (mp4) and will be preprocessed using openCV for conversion in individual frames.