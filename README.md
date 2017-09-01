# pyexcise

#遍历文件夹下所有文件
import os 
def Test1(rootDir): 
    list_dirs = os.walk(rootDir) 
    for root, dirs, files in list_dirs: 
        for d in dirs: 
            print（os.path.join(root, d)）
        for f in files: 
            print（os.path.join(root, f)）
