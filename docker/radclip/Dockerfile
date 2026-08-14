# Dockerfile for the RadCLIP foundation model.

FROM dockerdex.umcn.nl:5005/diag/base-images:base-pt2.7.1

ENV PIP_NO_CACHE_DIR=1

RUN python3 -m pip install --upgrade pip setuptools wheel

RUN python3 -m pip install --no-cache-dir \
    numpy==2.2.6 \
    pandas==2.2.3 \
    pydicom==3.0.1 \
    torch==2.7.0 \
    torchvision==0.22.0 \
    scikit-learn==1.6.1 \
    matplotlib==3.10.3 \
    transformers==4.52.0 \
    Pillow==11.2.1 \
    scipy \
    tqdm \
    monai[all]

ENTRYPOINT ["/bin/bash"]
