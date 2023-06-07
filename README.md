# bike-or-car
Example workflow of an object-detection deep learning model using fastai and gradio.

This is a product of putting my own spin on the fast.ai course (links below).

## Features
- Uses fastai libraries and gradio to train and deploy an object-detection model in Hugging Face Space.
- Dataset created from scratch by searching and downloading images using duckduckgo search library.
- The entire process can be done without running code locally and using free* resources.

## How to use the notebook
- Upload the notebook in Kaggle (Google Collab possible but not supported) and run the cells.
  - Alternatively copy and edit directly - https://www.kaggle.com/code/adbcode/bike-or-car.
- While the entire notebook can be run with a CPU instance, consider using a GPU instance for speedup in training.
- To run locally, it is recommended to setup a new Python environment of your choice with jupyter installed.

## To skip to creating your own gradio deployment
- Create `app.py` and `requirements.txt` as shown in the notebook.
- Download `model_XXX.zip.YYY` files corresponding to the image size of choice from this repository.
- Extract the archive alongside the above files.
- Ensure to rename the extracted file to `export.pkl` or modify the respective value in `app.py` in line 6 to match the name.
- Find an image each for a car or a bike and save them as `car.jpg` and `bike.jpg` respectively.
- Create your own Hugging Face Space and upload the above files to ensure it looks something like this - https://huggingface.co/spaces/adbcode/bike-or-car.

## Try deployed model
You can check out the model in action here - https://adbcode-bike-or-car.hf.space.
![image](https://github.com/adbcode/bike-or-car/assets/9251629/7a43105b-728e-49b9-81ea-74db88724d02)

## Reference
- https://www.kaggle.com/code/jhoward/is-it-a-bird-creating-a-model-from-your-own-data
- https://www.tanishq.ai/blog/gradio_hf_spaces_tutorial
