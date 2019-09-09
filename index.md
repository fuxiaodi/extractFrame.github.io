## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/fuxiaodi/extractFrame.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

# How to extract still images from a video?
## 1. use photoshop
### open photoshop, go to ->File, ->Open, -> select the .mov (a type of video format) file.
     ![Image](src=https://github.com/fuxiaodi/extractFrame.github.io/blob/master/file.png?raw=true)
### click the arrow ( in the lower left corner)
     ![Image](https://github.com/fuxiaodi/extractFrame.github.io/blob/master/file2.png?raw=true)
### set the parameters, see the following picture and click render.
      ![Image](https://github.com/fuxiaodi/extractFrame.github.io/blob/master/file3.png?raw=true)
### get still images in the folder which stores the original video.
      ![Image](https://github.com/fuxiaodi/extractFrame.github.io/blob/master/file4.PNG?raw=true)
      
      
## 2. use imutils (a python library) and openCV
### import imutils, codes: from imutils import FileVideoStream
### read the video: vs=FileVideoStream(path)
### write the codes: 
                   while True:
                       frame= vs.read()
                       frame=imutils.resize(frame,width=500)
                       cv2.imwrite(path,frame)









### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
