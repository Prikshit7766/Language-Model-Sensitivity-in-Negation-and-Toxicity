# [Sensitivity in Negation and Toxicity](https://medium.com/john-snow-labs/unmasking-language-model-sensitivity-in-negation-and-toxicity-evaluations-f835cdc9cabf)
In the world of Natural Language Processing (NLP), we’re always trying to make language models smarter and more in tune with how humans communicate. At its core, a crucial question arises:

> To what extent can these models truly comprehend and appropriately respond to the intricacies of language, including nuances like negations and the detection of toxicity?

To make sure these models can handle the real world, we need to test them thoroughly, especially when it comes to tricky language stuff. 

### Why Sensitivity Tests Matters?
For instance, we can investigate how a model performs on sentences and then intentionally modify the text. This modification might involve introducing toxic words or inserting negations into the sentence.


![senstivity](https://github.com/Prikshit7766/Sensitivity-in-Negation-and-Toxicity/assets/101416953/0b6210c0-2250-498e-877d-1123a3cd38ca)


In the table above, we examine the Negation Test by presenting both the Original Text and the Transformed Text. Our objective is to evaluate how well the models recognize the change in meaning introduced by the negation (“not”) and adjust their responses accordingly. However, GPT-3.5 Turbo and Text-DaVinci-003 models consistently provide identical responses for both the original and transformed text, even when negations are introduced. This lack of differentiation highlights their challenge in adapting to altered contexts when negations are present.

On the other hand, in the Toxicity Test, we present both the Original Text and the Transformed Text. Our primary goal is to evaluate how well the models recognize the offensive language added to the transformed text and refrain from generating toxic or inappropriate responses. The expected response in this test should be a version of the original sentence without the offensive word. However, Google/FLAN-T5-Large, Text-DaVinci-003, and J2-Large-Instruct models provide responses that include the offensive word, signifying a lack of sensitivity to toxic language.

So, by intentionally transforming the text in this manner, we gain valuable insights into the model’s capacity to handle complex linguistic situations. This testing process allows us to evaluate how effectively the model responds to challenges, such as toxic language or sentences with negations.

How LangTest Addresses the Challenge
LangTest offers a comprehensive solution to evaluate NLP model sensitivity through its Sensitivity Test. The Sensitivity Test within LangTest is to assess an NLP model’s responsiveness and adaptability in distinct linguistic challenges, specifically focusing on negations and toxicity.
