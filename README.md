# JMTS
- japanese manga translator using segmentation
- pre released colab version  
- 
# Result   
![result](doc/screenshot_1.png)    
![result](doc/screenshot_2.png)     
![result](doc/screenshot_3.png)    
![result](doc/screenshot_4.png)    



# Required environment to run  
- google ocr : google drive permission(credential file and scope file)
- window ocr : Microsoft.NET v4.0.30319,net core 3.1 runtime and window japanese ocr
- ez trans xp korea translator : ez trans xp program and ehnd 

# How to use  
- open the program and type manga site url then press enter
- It process translation (it takes time)
- it will create zip file on user's window download folder


# Supported URL
gallery-dl is used to download. Its support sites are:
- [supported site list](https://github.com/mikf/gallery-dl/blob/master/docs/supportedsites.rst)


# Workflow
- use gallery-dl to get managa from inputted url 
- do text segmentation from manga image using SickZil
- use opencv contour technique to detect text to crop text image based on text segmentation results
- get text from image using google ocr(or window ocr)
- convert japanese text to translated text using eztrans xp(or google translator)
- use pil to place translated text


# Run python
python gui.py  

# pip install 
pip install tensorflow-gpu==1.14.0   
pip install requests  
pip install PyQt5  
pip install tqdm funcy opencv-python Pillow  
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib  
pip install --upgrade pyinstaller==3.2.1  
pip install cefpython3  
pip install pywin32  
pip install matplotlib  
pip install imageio  
pip install google_trans_new  
pip install beautifulsoup4  
pip install wget  
pip install pyperclip  
pip install astor==0.8.0  
pip uninstall h5py  

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

