# News Headline Hallucination Detection Dataset

The dataset contains 6270 labeled examples for news headline hallucination detection used in the WebConf 2023 paper ""Why is this misleading?": Detecting News Headline Hallucinations with Explanations". ***News article titles and passages are included in this dataset***, they are extracted by the public [news-please](https://github.com/fhamborg/news-please) library based on the released article URLs. 

In particular, each row corresponds to one example and it contains the following six fields:
1. "ExampleId" field contains a unique identifier for this example.
2. "SplitID" field indicates which dataset split this example belongs to (one of
   train, validation, and test).
3. "ArticleURL" field includes the news article URL.  
4. "Generated Headline" field contains the generated news headline.  
5. **"ArticalTitle" field contains news titles extracted by the news-please library.**  
5. **"ArticalPassage" field contains news passages extracted by the news-please library.**  
7. "Explanation" field contains the human written explanation and could simply
   be an empty string.
8. "Label" field indicates if the headline is supported/entailed by the news
   article.


If you find this dataset useful for your research, please cite the following paper in your publication:

```
@inproceedings{Shen2023ExHalder,
  title={"Why is this misleading?": Detecting News Headline Hallucinations with Explanations},
  author={Jiaming Shen and Jialu Liu and Dan Finnie and Negar Rahmati and Michael Bendersky and Marc Najork},
  booktitle={Proceedings of The 34th International Conference in the Web (WWW 2023)},
  year={2023}
}
```
