# Py-FFT-Upscaling

Py-FFT-Upscaling is a Python application for upscaling images using Fast Fourier Transform (FFT) techniques, with a focus on safe memory usage and batch processing. It features a modern GUI built with CustomTkinter, allowing users to select input folders, output PDF destinations, and custom scaling factors for upscaling. The results, including upscaled images and their FFT spectra, are compiled into a PDF report.

## Features
- **Batch Image Upscaling:** Process all images in a folder at once.
- **FFT-Based Resizing:** Uses FFT for upscaling, preserving frequency information.
- **Safe Memory Handling:** Automatically downsamples large images to avoid out-of-memory errors.
- **Custom Scales:** Add multiple custom scaling factors for upscaling.
- **PDF Report Generation:** Outputs a PDF with original and upscaled images, FFT spectra, and processing notes.
- **Modern GUI:** Built with CustomTkinter for a user-friendly experience, including dark and light ("Modo Rosa") modes.

## Requirements
- Python 3.x
- numpy
- imageio
- matplotlib
- reportlab
- customtkinter
- pillow

Install dependencies with:
```bash
pip install numpy imageio matplotlib reportlab customtkinter pillow
```

## Usage
1. **Run the GUI:**
   ```bash
   python UI_FFT.py
   ```
2. **Select Input Folder:** Choose the folder containing images (JPG, PNG, BMP, etc.).
3. **Select Output PDF:** Choose where to save the generated PDF report.
4. **Add Scales:** Enter one or more scaling factors (e.g., 0.5, 2.0) and add them.
5. **Generate PDF:** Click "Generar PDF" to process images and create the report.

## File Structure
- `ProyectoFFT.py` — Core logic for FFT upscaling and PDF report generation.
- `UI_FFT.py` — CustomTkinter GUI for user interaction.
- `pink.json` — Theme file for the GUI (required for custom appearance).

## Notes
- The application is designed to avoid memory issues by capping image sizes and scaling factors.
- The GUI includes a fun "Modo Rosa" (pink mode) with a Hello Kitty background (image not included).
- All processing is done locally; no images are uploaded or sent to external servers.

## Authors
- Iker Garcia
- Das, Sara, Angel

## License
This project is for educational purposes. Please check with the authors for licensing if you plan to use it commercially or modify it for redistribution.
