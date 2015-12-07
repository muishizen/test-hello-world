# test-hello-world
The first work
# -*- coding: utf-8 -*-
import glob
import sys

#f = open('searching_result.txt','w')
#print 'WordNumber:'
#WordNum = sys.stdin.readline()
WordNum = '4024'
for file in glob.glob('/Users/Yusuke/Documents/共同研究/NUDriveData/NUDriveWord/*.word'):
      f = open(file, 'r')
      for line in f:
            #print line
            #line.decode('utf-8')
            #print 'line'+line+'\n'
            word = line.strip().split()
            #word = line.split() 
            #print word
            if WordNum in word:
                #print ('AAA\n')
                print file, ' : ', word.count(WordNum)
                #f.writelines(file+'¥n')
