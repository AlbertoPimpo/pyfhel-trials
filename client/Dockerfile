FROM pyfhel
COPY requirements.txt requirements.txt
RUN apt-get update && apt-get install libffi-dev
RUN pip3 install -r requirements.txt
COPY notebooks ./notebooks
ENTRYPOINT ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
