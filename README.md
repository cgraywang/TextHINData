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
