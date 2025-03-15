# Neural Style Transfer with PyTorch  

This project implements Neural Style Transfer (NST) using PyTorch and a pre-trained VGG19 model. The goal is to apply the artistic style of one image to another while preserving the content structure.  

## Features  
- Uses **VGG19** for feature extraction.  
- Supports **extreme style transfer tuning** for enhanced artistic effects.  
- Allows customization of **content and style weights**.  
- Saves the generated image after training.  

## Requirements  
Before running the code, install the required dependencies:  

```bash
pip install torch torchvision pillow
```

## Usage  

### 1. Prepare Your Images  
Place your **content image** and **style image** in the project directory. Update the file paths in the script:  

```python
content_path = r"your_content_image.jpg"
style_path = r"your_style_image.jpg"
```

### 2. Run the Script  
Run the following command to start the style transfer:  

```bash
python style_transfer.py
```

### 3. Output  
After training, the final image will be saved as `output.png`.  

## Customization  
- **Tuning Weights:**  
  Modify the `style_weight` and `content_weight` values for different artistic effects.  
- **Learning Rate:**  
  Adjust `lr` in the optimizer to control the speed of convergence.  
- **Epochs:**  
  Change the number of iterations to refine the output quality.  



## Future Improvements  
- Implementing Total Variation Loss for smoother results.  
- Adding a GUI for easier interaction.  

## License  
This project is open-source and available under the **MIT License**.  
