# Installing PyTorch in a Containerized Environment

To set up PyTorch in a containerized environment, you can use either `pip` or `conda` based on your preference and requirements. Here are the steps for both methods:

## Using `pip` (Recommended for Python virtual environments)

1. Activate your Python virtual environment if you haven't already:

   ```bash
   source <your_virtual_environment>/bin/activate

2. Install PyTorch and its related packages
   ```bash
   pip3 install torch torch vision torchaudio

3. Using `conda` (Recommended for Anaconda environments)

   If you haven't already, create a new anaconda environment(optional but recommended):
   ```bash
   conda create --name myenv python=3.8
   conda activate myenv
   
   Install PyTorch with CUDA support(adjust the 'pytorch-cuda' version as needed):
   ```bash
   conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
