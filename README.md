# LPI-MFF

LPI-MFF:Predicting lncRNA–protein interactions through deep learning framework  employing multiple features and random forest algorithm

# Requirements

Keras==2.2.5

matplotlib== 3.3.4

numpy ==1.19.5

tensorflow-gpu==1.14.0

pandas ==1.1.5

scikit-learn== 0.24.2

scipy==1.5.4

# NOTE

Before running main_fea.py, please get vectors of chemical and physical properties via the Pse-in-One-2.0 tool provided at http://bioinformatics.hitsz.edu.cn/Pse-in-One2.0/download/.

Use RPI1807 as an example:

python pse.py ./data/sequence/RPI1807_rdrna_seq.txt RNA PC-PseDNC-General -all_index ./data/pse/RPIRPI1807_rdrna_pse.txt

python pse.py ./data/sequence/RPI1807_rdprotein_seq.txt Protein PC-PseAAC-General -all_index ./data/pse/RPI1807_rdprotein_pse.txt

# How to run

```
cd ./sample
python main_fea.py -d 'RPI1807' -big_sel 0.8 -small_sel 0.9 -compe 15
```

