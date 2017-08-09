This is the groundtruth data for StampVar dataset (http://madm.dfki.de/downloads-ds-staver). 
In the original dataset, groundtruths for only stamp regions are available. 
We have generated pixel level groundtruth for non-overlapping regions. 
There is a text file named "images.txt", which contains all the image names for which the groundtruths are available. 


Groudtruth location = " /'resolution'dpi/groundtruth/'imagename'/ "

For a particular image, there are two files. One image file is "LabelAllInOne.png" which contains label of all regions in gray scale.
'255' denotes the background, and rest of the pixel information is in the 'inmageinfo.txt' file. 

'imageinfo.txt' file contains information in this format,

" LabelName	LabelNumber	NumberOfPB	NumberOfPixel "

where, 'Labelnumber' denotes the gray value of the pixel labeled as 'Labelname', and 'NumberOfPixel' denotes the number of pixels labeled with 'Labelname'.



For example: 

300dpi/groundtruth/stampDS-00201

imageinfo.txt ==>

LabelName	LabelNumber	  NumberOfPB  NumberOfPixel
  Text		0		24		446341
  Bold Text		1		1		4313
  Graphics		2		0		0
  Logo		3		1		44924
  Stamp		4		4		29506
  Headers		5		7		27863
  Head Line		6		0		0
  Signature		7		0		0
  Noise		8		3		2671


For example,

Labelname = "Text"  LabelNumber = "0" NumberOfPixel = "446341"

means, there is a labeled called "Text", it is represented as "0" gray value in "LabelAllInOne.png", and "446341" number of pixels are labeled as text in "LabelAllInOne.png". 


citation:




