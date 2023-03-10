# News Headline Hallucination Detection Dataset

The dataset contains 6270 labeled examples for news headline hallucination detection used in the WebConf 2023 paper ""Why is this misleading?": Detecting News Headline Hallucinations with Explanations". Each row corresponds to one example and it contains the following six fields:
1. "ExampleId" field contains a unique identifier for this example.
2. "SplitID" field indicates which dataset split this example belongs to (one of
   train, validation, and test).
3. "Generated Headline" field contains the generated news headline.
4. "ArticleURL" field includes the news article URL.
5. "Label" field indicates if the headline is supported/entailed by the news
   article.
6. "Explanation" field contains the human written explanation and could simply
   be an empty string.

Due to the policy constraints, we cannot directly provide the article titles and passages. However, you can use the public [news-please](https://github.com/fhamborg/news-please) library to extract the article contents based on the released article URLs. 

If you find this dataset useful for your research, please cite the following paper in your publication:

```
@inproceedings{Shen2023ExHalder,
  title={"Why is this misleading?": Detecting News Headline Hallucinations with Explanations},
  author={Jiaming Shen and Jialu Liu and Dan Finnie and Negar Rahmati and Michael Bendersky and Marc Najork},
  booktitle={Proceedings of The 34th International Conference in the Web (WWW 2023)},
  year={2023}
}
```
