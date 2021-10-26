# Turn-py-file-into-exec-Mac-
This is my 1st year to learn python. I am glad that I can turn my py file into an exec for others' using.

At first, you need prepare a py file which include some basic function.

Then, go as the below steps on your terminal.
1. Conda create --name office2 python=3.8 #build a new env(ex office2)，set 3.8v python
2. Conda activate office2 #attend new env
3. pip3 install pyinstaller
4. pip3 install (all the pip that target.py needed)
5. pip3 install --upgrade (all the pip that target.py needed) #Upgrade all the pips
6. pip3 install --force-reinstall --no-binary :all: pyinstaller #pyinstaller reinstall
7. mdfind -name "cv2" #find route for cv2
8. cd （route of target.py）
9. pyinstaller --onefile target.py --paths "/Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/cv2" #fix name of target.py，set the route from 7

Last edit date: 20211026
