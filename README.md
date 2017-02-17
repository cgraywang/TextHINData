# TextHINData
Text based heterogeneous information network datasets

20NG original data: 20news.data
Format:
doc id ||| category
content

20NG HIN: 20news.hin
Format of each document:
doc:doc id ||| category
(the parsing result of each sentence)
----sentence result:original sentence
（entity parsing result）
	entityID#1 entityType#1 entityInTheDoc#1
	...
	...
	entityID#n entityType#n entityInTheDoc#n
（relation parsing result, level=1 (relation in the doc)，level=2(relation in the knowledge base)）
		subjectID    predicate    objectID    level
		...
		...
		...

References:
@inproceedings{wang2015world,
 author = {Wang, Chenguang and Song, Yangqiu and El-Kishky, Ahmed and Roth, Dan and Zhang, Ming and Han, Jiawei},
 title = {Incorporating World Knowledge to Document Clustering via Heterogeneous Information Networks},
 booktitle = {KDD},
 isbn = {978-1-4503-3664-2},
 location = {Sydney, NSW, Australia},
 pages = {1215--1224},
 year = {2015},
} 
@inproceedings{wang2016text,
  title={Text Classification with Heterogeneous Information Network Kernels.},
  author={Wang, Chenguang and Song, Yangqiu and Li, Haoran and Zhang, Ming and Han, Jiawei},
  booktitle={AAAI},
  pages={2130--2136},
  year={2016}
}
