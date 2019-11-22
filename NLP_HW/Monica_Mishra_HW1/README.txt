################
All questions have been implemented in Python
Code requires Jupyter notebook to run and check the results properly
################

################
Q1

Run each cell and all the probabilities will listed.

Answer: {'D1': 'fruit', 'D2': 'vegetable'}

Probabilities: 
D1 = {'vegetable': 3.522258934549205e-08, 'flower': 5.85199329043067e-07, 'fruit': 1.8635701033660223e-05}
D2 = {'vegetable': 1.5533161901361992e-05, 'flower': 1.0552774786022522e-07, 'fruit': 1.5401405812942332e-07}
################

################
Q2

Run each cell and the number of word sense for each word will appear.

Answer:

2.1 ---> {'in': 7, 'the': 0, 'cold': 16, 'weather': 6, 'they': 0, 'started': 14, 'to': 0, 'city': 3, 'were': 13, 'least': 12, 'worried': 8, 'protecting': 3, 'themselves': 0, 'against': 0, 'common': 10, 'after': 3, 'she': 0, 'signed': 10, 'agreement': 6, 'a': 7, 'chill': 7, 'crept': 4, 'up': 14, 'her': 0, 'spine': 5, 'its': 1, 'not': 1, 'that': 0, 'serious': 6, 'husband': 2, 'assured': 8, 'and': 0, 'left': 24, 'deposit': 12, 'cash': 4, 'at': 2, 'bank': 18}

2.2 ---> {'in': 7, 'the': 0, 'cold': 16, 'weather': 6, 'they': 0, 'start': 22, 'to': 0, 'city': 3, 'were': 13, 'least': 12, 'worry': 8, 'protect': 2, 'them': 0, 'against': 0, 'common': 10, 'after': 3, 'she': 0, 'sign': 20, 'agree': 7, 'a': 7, 'chill': 7, 'crept': 4, 'up': 14, 'her': 0, 'spine': 5, 'it': 1, 'not': 1, 'that': 0, 'serious': 6, 'husband': 2, 'assure': 6, 'and': 0, 'left': 24, 'deposit': 12, 'cash': 4, 'at': 2, 'bank': 18}
################

################
Q3

In the data extractor function just provide the dataset name and ensure it is on the same directory as the script
Possible argument for data extractor function = "gutenberg", "imdb_data", "news_data"

Run each cell to get the count. Showing some counts here for the purpose of simplicity and please find the average perplexity value for both test datasets.

Part 3.1 ---->
Three grams: 
Counter({'[ emma by': 1,
         'emma by jane': 1,
         'by jane UNK': 3,
         'jane UNK UNK': 7,
         'UNK UNK ]': 23,
         'UNK ] volume': 1,
         '] volume i': 1,
         'volume i chapter': 1,
         'i chapter i': 1,
         'chapter i emma': 2,
         'i emma woodhouse,': 1,
         'emma woodhouse, handsome,': 1,
         'woodhouse, handsome, clever,': 1,
         'handsome, clever, and': 1,
         'clever, and rich,': 1,
         'and rich, with': 1,
         'rich, with a': 1,
         'with a comfortable': 1,
         'a comfortable home': 2,............................})


Four grams:
Counter({'[ emma by jane': 1,
         'emma by jane UNK': 1,
         'by jane UNK UNK': 3,
         'jane UNK UNK ]': 3,
         'UNK UNK ] volume': 1,
         'UNK ] volume i': 1,
         '] volume i chapter': 1,
         'volume i chapter i': 1,
         'i chapter i emma': 1,
         'chapter i emma woodhouse,': 1,
         'i emma woodhouse, handsome,': 1,
         'emma woodhouse, handsome, clever,': 1,
         'woodhouse, handsome, clever, and': 1,
         'handsome, clever, and rich,': 1,
         'clever, and rich, with': 1,
         'and rich, with a': 1,
         'rich, with a comfortable': 1,
         'with a comfortable home': 1,
         'a comfortable home and': 1,
         'comfortable home and happy': 1,
         'home and happy disposition,': 1,
         'and happy disposition, seemed': 1,............................})


Part 3.2 ---->
Average perplexity for imdb_data dataset: 70.17773402921019
Average perplexity for news_data dataset: 128.4372991933948
################



################
Q4

In the data extractor function just provide the dataset name and ensure it is on the same directory as the script
Possible argument for data extractor function = "brown-copy"

Run each cell to get the count. Showing some counts here for the purpose of simplicity and please find the average perplexity value for both test datasets.

4.1 --->
Reporting only a few quantities
word_tag counts:  
Counter({'<START>': 48577,
         'The/at': 7187,
         'Fulton/np': 17,
         'County/nn': 85,
         'Grand/jj': 15,
         'UNK/nn': 14629,
         'said/vbd': 1697,
         'Friday/nr': 59,
         'an/at': 3496,
         'investigation/nn': 42,
         'of/in': 35757,
         's/np': 2594,
         'recent/jj': 167,
         'primary/nn': 17,
         'election/nn': 74,
         'produced/vbd': 28,
         'no/at': 1536,
         'evidence/nn': 199,
         'that/cs': 6346,
         'any/dti': 1271,
         'irregularities/nns': 8,
         'took/vbd': 418, .............................})

tag_counts:
Counter({'<END>': 48577,
         '<START>': 48577,
         'Output': 4,
         'abl': 353,
         'abn': 2957,
         'abx': 728,
         'active': 1,
         'ap': 9476,
         'at': 98031,
         'be': 6294,
         'bed': 3247,
         'bedz': 9765,
         'beg': 675,
         'bem': 230,
         'ben': 2432,
         'ber': 4420,
         'bez': 10169,.............................})


bi_gram_counts:
Counter({'<START> at': 7616,
         'at np': 3024,
         'np nn': 4888,
         'nn jj': 2257,
         'jj nn': 31102,
         'nn vbd': 4399,
         'vbd nr': 113,
         'nr at': 89,
         'at nn': 52459,
         'nn in': 46270,
         'in np': 8512,
         'np jj': 843,
         'nn nn': 17363,
         'vbd at': 3962,
         'nn cs': 4600,
         'cs dti': 224,
         'dti nns': 378,
         'nns vbd': 1669,
         'vbd nn': 608,
         'nn <END>': 20572,.......................})

Part 4.2 ---->
Transition Probability:
{'<START> at': 0.1567492251141233,
 'at np': 0.030845006925617438,
 'np nn': 0.13014180054206892,
 'nn jj': 0.013538283995062374,
 'jj nn': 0.4589713243453828,
 'nn vbd': 0.026386188083239066,
 'vbd nr': 0.004405612384016703,
 'nr at': 0.04505005561735261,
 'at nn': 0.5350687155886571,
 'nn in': 0.27753212275926437,
 'in np': 0.07020010754213442,
 'np jj': 0.022446871389091527,
 'nn nn': 0.1041453984469751,
 'vbd at': 0.15433666513450556,
 'nn cs': 0.027591803732969933,.......................})

Part 4.3 ------>
Emission Probability:
{'The/at': 0.07181598895246241,
 'Fulton/np': 0.00043187707414647455,
 'County/nn': 0.0005042825499275279,
 'Grand/jj': 0.000216333617957696,
 'UNK/nn': 0.08668859989594357,
 'said/vbd': 0.06125255354319909,
 'Friday/nr': 0.014728604894582066,
 'an/at': 0.03493424037187514,
 'investigation/nn': 0.0002494746809864738,
 'of/in': 0.2900252738268272,
 's/np': 0.06551650982709764,
 'recent/jj': 0.0023939965272007286,
 'primary/nn': 0.00010133057113702383,
 'election/nn': 0.00043909914159376984,................})


Part 4.4---->
Result of 5 random sentences:
Sentence ID: 1 
	 John/np 0.0007098881965105562 William/np 0.0007291966409498122 of/in 0.018772209734886754 the/at 0.22266728573686068 grounds/nns 6.915242320338724e-05 of/in 0.07908709712941428 all/abn 0.00434994068179207 be/be 0.001543369745140279 with/in 0.002340103095761513 both/abx 0.0004348187807154439 The/at 0.007202984273656557 spite/nn 0.00015251024398632337 and/cc 0.05789187326335965 it/pps 0.007095342160281965 was/bedz 0.12110602133238504 implying/vbg 3.072770558043864e-05 

**Printing the sentence properly**
	 John William of the grounds of all be with both The spite and it was implying 

Sentence ID: 2 
	 who/wps 0.0005389002024534835 get/vb 0.0021519696210883033 his/pp 0.01681628796631599 British/jj 0.0002648576310265283 to/to 0.016668149746310208 understand/vb 0.0030966175475128834 Hanover/np 3.354784438502727e-05 

**Printing the sentence properly**
	 who get his British to understand Hanover 

Sentence ID: 3 
	 shaking/vbg 1.1680090182855517e-05 to/in 0.014613290979083142 an/at 0.012544165832738008 fault/nn 7.007227426398642e-05 Af/nn 0.0006134999614596458 in/in 0.04259250616386392 my/pp 0.003775854381929988 underlying/vbg 1.22435097533252e-05 the/at 0.08751171742724961 bit/nn 0.0002951913454288296 started/vbd 0.00012961388976376881 in/in 0.0264836077185481 the/at 0.22266728573686068 scientific/jj 0.0002568684921572241 existence/nn 0.0002940056162127484 

**Printing the sentence properly**
	 shaking to an fault Af in my underlying the bit started in the scientific existence 

Sentence ID: 4 
	 batch/nn 1.2309915162205632e-06 with/in 0.015622572262068908 his/pp 0.021268098181163597 countries/nns 0.00048136309436081875 

**Printing the sentence properly**
	 batch with his countries 

Sentence ID: 5 
	 this/dt 0.012057133216562493 will/nn 0.00029922984169964355 as/cs 0.0063515204078663755 the/at 0.1608102470389059 fair/jj 0.00018577372296810072 Supreme/jj 2.8185444401170853e-05 interview/nn 8.458440947471301e-05 with/in 0.015622572262068908 some/dti 0.0025107336782454366 symbol/nn 0.00013181722758083935 

**Printing the sentence properly**
	 this will as the fair Supreme interview with some symbol
      

Part 4.5 ----?

In the collect dataset function provide the location of the test dataset (a separate function was created since the parsing was different).

Output file has been attached with the code.