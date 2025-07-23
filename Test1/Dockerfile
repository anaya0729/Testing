FROM jupyter/base-notebook

# Set working directory
WORKDIR /home/jovyan/Test1

# Optional: install more Python packages
RUN conda install -y pandas matplotlib seaborn

CMD ["start-notebook.sh","--NotebookApp.token=''", "--NotebookApp.password=''"]