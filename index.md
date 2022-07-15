## By: Shreyas, Phillip, Aidan, Maahir

## Identifying Genders of Authors in the 1600s

What exactly did we do? Well the first thing we did was try and identify different features that we could use. To do that, we wanted to know exactly what separates the writing styles of men and women. After brainstorming, we came to several conclusions. We saw that there was a greater use of pronouns in the women's texts compared to the men's texts. Not only did we find a correlation in the use of pronouns, but also in the use of logical connectors like "therefore" and "hence". We saw that these words were used more frequently in the men's texts. One last thing that we noticed was the use of punctuation. Since the women's sentences were generally longer they also contained more punctuation. 

Now that we figured out some of the features we wanted to use, what do we do with them. At first we thought that all we really needed was a "Bag of Words", but we soon came to realize that "Bag of Words" doesn't cover punctuation. So we needed to adjust our model. We used a count function to find the frequencies of all the words and punctuation. After that we decided not to use KNN or SVM models since we felt that those two didn't really have any learning going on, we decided to use a perceptron model. Now if the weights returned are negative then it is indicative of the males writing style, and a positive weight is indicative of female writing style.

The weights we recieved are: [-54,  -322,   318,  2588, -1897,  1802, -4925,    48,  2578, -2821,  -260,  -187,   784,  -128,  1759] <br>
The new bias is: -876 <br>
The validation accuracy is: 80%  <br>
The testing accuracy is: 98.7%

<body>
        <div class = "center">
            <h3>View Our Code!</h3>
            <script src="https://gist.github.com/shreyas-s125/74bdb14a1dafab9619a30c08c73ff714"></script>
        </div>
    </body>  




