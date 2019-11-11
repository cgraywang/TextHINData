# A [text-to-network representation](https://github.com/cgraywang/TextHIN) based datasets

# Data format:

## 20NG.data.zip: 20 newsgroups dataset

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

## GCAT.data.zip: RCV1 GCAT category dataset

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
We released our [[source code]](https://github.com/cgraywang/TextHIN) for the "Knowsim: A document similarity measure on structured heterogeneous information networks". Other source code would be released.

## References:

        @article{wang2018unsupervised,
        title={Unsupervised meta-path selection for text similarity measure based on heterogeneous information networks},
        author={Wang, Chenguang and Song, Yangqiu and Li, Haoran and Zhang, Ming and Han, Jiawei},
        journal={Data Mining and Knowledge Discovery},
        volume={32},
        number={6},
        pages={1735--1767},
        year={2018},
        publisher={Springer}
        }
        
        @inproceedings{wang2017distant,
        title={Distant meta-path similarities for text-based heterogeneous information networks},
        author={Wang, Chenguang and Song, Yangqiu and Li, Haoran and Sun, Yizhou and Zhang, Ming and Han, Jiawei},
        booktitle={Proceedings of the 2017 ACM on Conference on Information and Knowledge Management},
        pages={1629--1638},
        year={2017},
        organization={ACM}
        }
        
        @article{wang2016world,
        title={World knowledge as indirect supervision for document clustering},
        author={Wang, Chenguang and Song, Yangqiu and Roth, Dan and Zhang, Ming and Han, Jiawei},
        journal={ACM Transactions on Knowledge Discovery from Data (TKDD)},
        volume={11},
        number={2},
        pages={13},
        year={2016},
        publisher={ACM}
        }
        
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
