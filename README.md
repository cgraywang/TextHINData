# TextHINData
# Knowledge Graph Augmented Text as Heterogeneous Information Network (HIN) datasets


# Data format:

## 20NG.data.zip: [20 newsgroups dataset](http://qwone.com/~jason/20Newsgroups/)

Format:
        
        documentID ||| category
        content

## 20NG.hin.zip: 20 newsgroups HIN dataset based on semantic parsing from Freebase

Format:
        
        documentID ||| category
        
        (Entities and relations (with the type information) parsed from each sentence of the document)
        
        ----sentence result: sentence
        
        (Entities)
        
        entityID#1 entityType#1 entity#1
        
        ...
        
        ...
        
        entityID#n entityType#n entity#n
        
        (Relations)
        
        (indicator=1 (relation from the document), indicator=2 (relation from Freebase))
        
        subjectEntityID    relation    objectEntityID    indicator
        
        ...
        
        ...
        
        ...

## GCAT.data.zip: [RCV1 GCAT category dataset](http://www.daviddlewis.com/resources/testcollections/rcv1/)

Format:
        
        same as 20NG.data.zip

## GCAT.hin.zip: RCV1 GCAT category HIN dataset based on semantic parsing from Freebase

Format:
        
        same as 20NG.hin.zip

## Usage:
  
  Unzip the according dataset.


# Construction details:

  Please refer to the following papers.
  
# How to Use the Text based Heterogeneous Information Network Datasets:
We released our source code for the "Knowsim: A document similarity measure on structured heterogeneous information networks" [code](https://github.com/cgraywang/TextHINData). Other source code would be released.

## References:

        @inproceedings{wang2016text,
        title={Text Classification with Heterogeneous Information Network Kernels},
        author={Wang, Chenguang and Song, Yangqiu and Li, Haoran and Zhang, Ming and Han, Jiawei},
        booktitle={AAAI},
        pages={2130--2136},
        year={2016}
        }

        @inproceedings{wang2015knowsim,
        title={Knowsim: A document similarity measure on structured heterogeneous information networks},
        author={Wang, Chenguang and Song, Yangqiu and Li, Haoran and Zhang, Ming and Han, Jiawei},
        booktitle={2015 IEEE International Conference on Data Mining},
        pages={1015--1020},
        year={2015},
        organization={IEEE}
        }

        @inproceedings{wang2015world,
        author = {Wang, Chenguang and Song, Yangqiu and El-Kishky, Ahmed and Roth, Dan and Zhang, Ming and Han, Jiawei},
        title = {Incorporating World Knowledge to Document Clustering via Heterogeneous Information Networks},
        booktitle = {KDD},
        pages = {1215--1224},
        year = {2015}
        }

