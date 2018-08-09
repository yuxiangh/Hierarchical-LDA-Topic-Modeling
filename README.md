# Hierarchical-LDA-Topic-Modeling(Python3 Version) 
Created the Hierarchical LDA topic modeling algorithms based on penalized average cosine similarity algorithms


Implement the Hierarchical LDA topic modeling algorithmsc based on penalized avergae coisine similarity methods created by Yuxiang Hou  

Problem desciption- LDA topic modeling algroithm always have a hard time to get the number of topic.This Algorithm will automatically get the correct number of topics based on average cosine similarity.    

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

Utilized Tableau To visualize the Hierarchical LDA output results:

Depth one:  

![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth%201.png) 



Depth Two:
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth2.png)   


Depth Three:   
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth3.png)   

Depth Four:
![alt text](https://github.com/yuxiangh/Hierarchical-LDA-Topic-Modeling/blob/master/HLDA%20Visualiztion/depth4.png) 




















