FROM pyfhel
RUN pip3 install requirements.txt
COPY notebooks ./notebooks
WORKDIR notebooks
ENTRYPOINT ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
