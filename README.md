Here’s the README in an editable text format:

---

# Facial Emotion Recognition using Semi-Supervised Neural Networks

This project implements methods from the paper *"Analysis of Semi-Supervised Methods for Facial Expression Recognition"* presented at the 2022 ACII Conference. The project explores semi-supervised learning techniques for facial emotion recognition.  

## Project Structure  

- **Code Files**:  
  - `train_utils.py`: Training utility functions.  
  - `uda.py`: Unsupervised Data Augmentation.  
  - `utils.py`: General utility functions.  
  - `vat.py`: Virtual Adversarial Training implementation.  
  - `custom_writer.py`: Logging and custom writer utilities.  
  - `eval.py`: Evaluation pipeline.  
  - `fixmatch.py`, `fullysupervised.py`, `meanteacher.py`, `mixmatch.py`, `pimodel.py`, `pseudolabel.py`, `remixmatch.py`: Implementations of semi-supervised learning methods.  

- **Folders**:  
  - `models/`: Predefined neural network architectures.  
  - `datasets/`: Dataset loading and preprocessing.  
  - `config/`: Configuration files for model training and evaluation.  

## Running the Project  

1. **Dependencies**: Install required Python packages listed in `requirements.txt`. Use:  
   ```bash
   pip install -r requirements.txt
   ```

2. **Dataset Preparation**:  
   Place your facial emotion datasets in the `datasets/` folder. Update the preprocessing scripts as needed.  

3. **Training**:  
   To train a model, use one of the provided methods (e.g., FixMatch, Mean Teacher):  
   ```bash
   python fixmatch.py --config config/fixmatch_config.json
   ```  

4. **Evaluation**:  
   Evaluate trained models using:  
   ```bash
   python eval.py --model_path <path_to_trained_model>
   ```  

---
