# JMTS
- japanese manga translator using segmentation([Unconstrained Text Detection in Manga](https://github.com/juvian/Manga-Text-Segmentation))
- pre released colab version  
- 
# Result   
![result](doc/screenshot_1.png)    
![result](doc/screenshot_2.png)     
![result](doc/screenshot_3.png)    
![result](doc/screenshot_4.png)    



# Supported URL
gallery-dl is used to download. Its support sites are:
- [supported site list](https://github.com/mikf/gallery-dl/blob/master/docs/supportedsites.md)


# Workflow
- use gallery-dl to get managa image from inserted url 
- do text segmentation([Unconstrained Text Detection in Manga](https://github.com/juvian/Manga-Text-Segmentation)) on manga image
- use opencv contour technique to detect text to crop text image based on text segmentation results
- recognise text using ocr(google ocr or tesseract ocr)
- convert japanese text to translated text using translator(google translate)
- use pil to place translated text


# Run python
python gui.py  

# pip install   
pip install tqdm opencv-python Pillow  
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib  
pip install --upgrade pyinstaller==3.2.1  
pip install cefpython3  
pip install pywin32  
pip install matplotlib  
pip install google_trans_new  
pip install beautifulsoup4  
pip install wget  
pip install pyperclip  

or  
conda remove --name py35 --all  
conda create --name py35 python=3.5  
activate py35  
pip install -r requirements.txt  
pip freeze > requirements.txt  


# Acknowledgement and References  
- [Unconstrained Text Detection in Manga](https://github.com/juvian/Manga-Text-Segmentation)
- [Telea Inpaint](https://docs.opencv.org/3.4/df/d3d/tutorial_py_inpainting.html  )
- [Biharmoic inpaint](https://scikit-image.org/docs/dev/auto_examples/filters/plot_inpaint.html)
- [PatchMatch inpaint](https://github.com/vacancy/PyPatchMatch.git)
- [gallery-dl](https://github.com/mikf/gallery-dl)  
- [Tesseract](https://github.com/tesseract-ocr/tesseract)  
- [Pytesseract](https://pypi.python.org/pypi/pytesseract)  
- [nhocr](https://github.com/fireae/nhocr)  
- [google drive](https://developers.google.com/drive/api/v3/quickstart/python)  
- [google_drive_ocr](https://tanaikech.github.io/2017/05/02/ocr-using-google-drive-api/)
- [window10_ocr](https://medium.com/rkttu/using-windows-10-built-in-ocr-with-c-b5ca8665a14e)
- [OpenCV with Python wrapper](https://pypi.org/project/opencv-python/)  
- [text-detection](https://github.com/qzane/text-detection)  
- [Google Translate API for Python](https://pypi.org/project/googletrans/)  
- [google translate new](https://github.com/lushan88a/google_trans_new)  
- [ehnd](https://github.com/sokcuri/ehnd)  
- [ezTransWeb](https://github.com/HelloKS/ezTransWeb)
- [cefpython](https://github.com/cztomczak/cefpython)  

