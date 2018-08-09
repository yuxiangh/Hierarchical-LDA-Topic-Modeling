# Hierarchical-LDA-Topic-Modeling(Python3 Version)


# BackGround  
Topic Modeling is Always a popular way to know what's people are talking about. But how to get the correct number of topics is always a tricky problem in LDA topic modeling. This algorithm created by Mayank, Yuxiang Hou From Information Science Institute.It was mainly to solve the problem of how to get correct number of topics in traiditonal LDA topic modeling and get overviews and details of what people are talking about.The Main idea is to run LDA topic model in corpus, and get the number of topics based on lowest avergae cosine similarity. And then run the LDA topic model in each sub topic, in this way, it will create the hierarchical tree structured topic modeling. 


# Algorithms Details
1.Created the Auto-LDA topic modeling algorithms based on penalized average cosine similarity algorithms.(Auto LDA is a algorithm created by Yuxiang Hou to get the correct number of topics based on lowest average cosine similarity bacause the less the overlapping topics model, the better the result is).    

2.Utilized BFS algorithm to get each layer tree sub topics. And for these sub topics, run the Auto-LDA again util the tree depths reach 5 or the topic meaning is not relevant to disasters. 



# Output   
This programs otuput will produce a dataset, For each sentence it will have the First/Second/Third/Fourth Topic meaning. In that way, people can know the main topic and details.  Then we can utilize the Tableau Treemap to visualize the results like below. 





# Configuration set up
packages in this algorithm: ntlk, numpy, pandas, pprint, gensim, pyLDAvis, matplotlib, spacy 

pip3 install nltk  
pip3 install numpy   
pip3 install panda  
pip3 install gensim    
pip3 install pyLDAvis    
pip3 install matplotlib   
pip3 install spacy 


# Run programs on Command line  
four parameters need to be set up after programs running:   
1. Json line path which includes all the single json files 
2. Lexicon json path     
3. Id path in the single json files.        
4. Sentence path in the single json files.       


Explaniation of input parameters of Id path and Sentence Path in a single json file:   
Example:
{key1:{"Id":12345},key2:{"Sentence":"this programs is aweseome"}}  


Id path is "key1.Id"  
Sentence path is "key2.Sentence"
(utilized the "." to connect the sequence of the path)


# Command line Running Example

python3 /Users/yuxianghou/Desktop/HLDA.py





# Visulization Result:

Utilized Tableau treemap To visualize the Hierarchical LDA output results:

Depth one:  

![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth%201.png) 



Depth Two:
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth2.png)   


Depth Three:   
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth3.png)   

Depth Four:
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth4.png) 




















