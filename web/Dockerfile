FROM python:3.6.9
RUN pip install --upgrade pip
#RUN pip --no-cache-dir install https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow_gpu-2.1.0-cp36-cp36m-manylinux2010_x86_64.whl
WORKDIR /usr/src/app
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD [ "python", "app.py" ]
