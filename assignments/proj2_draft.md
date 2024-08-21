::: title
The State of Generative AIs: A Narrative Review
:::

::: authors
Hendra Anggrianto Wijaya<br>A20529195<br>*Illinois Institute of Technology*<br>hwijaya@hawk.iit.edu
:::

::: content
**_Abstract_&mdash;Recent advancements in natural language processing have
allowed AI models to digest massive datasets, making it possible to appear
human-like by imitating our intelligence to a compelling degree. This newfound
phenomenon accelerates a public perception that the dawn of AI is nigh. In this
paper, I look at different AI models and how they perform in their respective
fields. The review is conducted in the spirit of story-telling in place of
hard-hitting scientific findings.**

**_Index Terms_&mdash;generative AI, chat bots, artificial intelligence, LLM,
LDM**

## I. Introduction

The desire for automating human tasks is nothing new, with the first recorded
design dating back to 1832, but perhaps first popularized with the publication
of the Turing Test by Alang Turing in 1950.\[1\] However, it wasn't until the
late 1980s that there is a breakthrough with a collective study into neural
networks, an adaptable decision-making system inspired by the human brain.\[2\]
All this brief history contributes to the current state of the Natural Language
Model (NLP), where it is now possible to process large quantities of data far
surpassing human capabilities.

## II. Comparison of Content

Since its public release in late 2022, *OpenAI*'s *ChatGPT* has broken new
ground on what is possible with chatbots and captured the world's attention. It
prompted *Google* to react by releasing their version of chatbots in early 2023,
named *Bard*. In this section, I will attempt to compare these two chatbots as
the current frontier of text-based generative AIs. As a collateral study, I will
also discuss other forms of content that modern generative AIs can produce, such
as code and images.

### A. Text

Unsurprisingly, plain text content generation has garnered the most adoption
because of its high potential findings with relatively low requirements, which
can be a skill or economic barrier. ChatGPT and Bard remain free for evaluation
at the time of the writing, which may very well contribute to their massive
popularity. Nowadays, we have found ways to integrate them into our lives,
producing countless homework, resumes, and other work documents.

At the core of ChatGPT is a proprietary GPT, a language model tailored for more
innovative conversations.\[3\] Its creative upbringing makes it suitable for
generating non-formal letters but can turn frustrating advanced on topics as it
lacks higher contextual awareness. The notion of creativity itself can backfire,
for example, as users expect out-of-the-box answers from ChatGPT, it is safe to
presume most answers do not satisfy their requirements.

In direct contrast, Bard can produce a more comprehensive understanding but
appears less innovative by design. Thus feasible for scientific needs like
analysis reports and academic papers. In addition, Bard is at the advantage of
being maintained by Google, the biggest search engine for limitless data-feeding
prospect, as opposed to ChatGPT which is still capped at 2021 knowledge.

### B. Code

ChatGPT and Bard are capable of producing code, albeit chaotically as code
requires more precision and detailed problem descriptions than natural
language.\[4\] They are the perils of scourging online source code without
adequate context, bad sources are bound to be embraced as incorrect ground
truths. It is difficult to say whether large language models (LLM) can solve the
issue in the foreseeable future, but conventional thinking suggests that they
are still in early development and there is room to improve.

Much to developers' disdain, *GitHub Copilot* was released in 2022 as paid
service to alleviate some writing tasks with AI.\[5\] GitHub Copilot is also an
LLM and suffers from the same deficiency ChatGPT and Bard have. However, if we
are to measure code-synthesis LLMs by usability, Copilot stands out for its
seamless integration with IDE.

```python
from typing import List

def has_close_elements ( numbers : List [ float ] , threshold :
  float ) -> bool :
  """ Check if in given list of numbers , are any two
   numbers closer to each other than given threshold .
  >>> has_close_elements ([1.0 , 2.0 , 3.0] , 0.5)
  False
  >>> has_close_elements ([1.0 , 2.8 , 3.0 , 4.0 , 5.0 , 2.0] , 0.3)
  True
  """
  for i in range (len( numbers ) ) :
    for j in range ( i + 1 , len( numbers ) ) :
      if abs( numbers [ i ] - numbers [ j ]) < threshold :
        return True
  return False
```

<small>Figure 1 &mdash; Example of GitHub Copilot suggestion (in string)</small>

### C. Art

Synthesizing images requires a different toolset that conventional LLMs lack.
The current working model is diffusion, that is, repeatedly adding noise to the
image and diluting them with a trained decoder, resulting in a reconstructed
image that resembles the original version.\[6\] *DALL-E* is one of the first to
use diffusion techniques since its introduction by OpenAI in late 2021. Today,
DALL-E is known to generate photo-realistic images indistinguishable from
reality.

Late discoveries branded latent diffusion models (LDM) pushes efficiency and
overall quality but at the cost of increased complexity, adopted by *Stable
Diffusion* and *Midjourney*.\[7\] In my limited study, Stable Diffusion produces
natural images with less noise while Midjourney is geared towards surreal images
with artistic values.

It is inherently difficult to measure accuracy in AI-generated images due to the
high subjectivity of the objects they potray. Nevertheless, one research that
limits the testing scope to strictly human faces found that images fabricated by
Stable Diffusion are the most credible. Furthermore, the study notes that
results that are too graphically pleasing could be discouraging and provokes an
accusation of being fake.

![](https://github.com/hanggrian/IIT-CS487/raw/assets/assignments/proj2/fig1.png)

<small>Figure 2 &mdash; Comparison of Stable Diffusion, Midjourney, and DALL-E</small>

## III. Engineering of Chatbots

These generative AIs work by analyzing the compositions of user input and
comparing them with accumulated training data. Depending on the input difficulty
and the dataset size, the AIs then predict output materials utilizing various
neural networks.

### A. Awareness

In the context of AI, being aware refers to the ability to sense the environment
and react accordingly, rather than consciousness typically associated with human
compassion. Considering AI models use their judgment to devise decisions, few
are bound to be defective, even more so in early training drills or when the AI
model tries the shoot-for-the-star approach.

A range of developer interventions such as changing training routines and
filtering errors can reduce the flaws in generated content. But just as the AI
models could be guided to minimize deficiency, they are also susceptible to
manipulation by bad actors. AIs can practically be fed biased data to
intentionally wreak havoc in their environment unless there is a safeguard to
prevent it.

### B. Consciousness

Contrary to the popular belief that AI models are sentient, the capability of
generative AIs is restricted to recognizing patterns and predicting the most
probable outcome. Simply put, AIs lack sympathy even if the content they
generate appears to be empathetic. There is no scientific evidence that
indicates otherwise.

Nonetheless, it is theoretically possible to program consciousness into AI
models, presuming that being conscious refers to common sense instead of
biological systems.\[8\] Following up on an example from the previous section
where AIs occasionally produce defects, they can be coached to feel remorse and
take them into account for the next decision. It could also backfire, in
particular, when the AIs use their emotions as justification for poor deeds.

## IV. Evaluation of Impact

Although artificial intelligence and deep learning technologies are still in
their infancy, they have had a profound impact on scientific fields and are
projected to rise in the years to come.\[9\] AI development has opened up new
fields of study like automated vehicles, virtual assistants, and professional
tools. On top of that, bringing innovations can help create or impact existing
markets unrelated to AI.

Having said that, the specific fields in which they excel do not necessarily
translate to direct economic retributions or policy changes. Whereas AI models
will inevitably create opportunities, further evaluation is required to learn
the detailed economic impact and the business model essential to sustain the
operations.

### A. Liability

For so long in software products and services, the burden of accountability lies
on the software provider or maintainer. Case in point, an early record of
Oklahoma Law Review in 1980 has put in writing that anyone who profits from the
product is solely liable for any harm inflicted upon the user or his/her
property.\[10\] Be that as it may, the conversation gets trickier with
generative AIs because we are introducing new actors into the equation.

There are several propositions to mitigate the AI liability concern. Perhaps
none more popular than a publication by criminal law professor Gabriel Hallevy,
which emphasizes responsibility on the trainers as well as the programmers.\[11\]
The users are also somewhat at risk with this model, though the settlement is
likely to be on a case-to-case basis.

### B. Reliability

The question of trustworthiness arises as more AIs will be incorporated into our
daily lives, particularly, whether or not humans should put absolute confidence
in automated machines. The seriousness of such a claim cannot be underestimated
as we tend to value trust as defining human attributes.

At the heart of the argument, there is no scientific consensus that states AI
holds the characteristics required to be considered trustworthy. AI models make
decisions systematically, and thus should not be relied upon on a personal
extent.\[12\] The faith, if any, should instead be directed into AI's habitual
routine.

## V. Case Study

On a quiet day in March 2016, a naive division at *Microsoft* released their
chatbot to *Twitter* in the persona of a young teenage girl named *Tay*.\[13\]
The launch initiated substantial excitement among Twitter users, as indicated by
unusually high traffic within the same period. The initial idea was noble
enough, that is, to provide Tay with a self-learning ability to assess tweets
from the general public.

However, without sufficient supervision, it does not take long for the whole
system to fall apart. In just a day after its deployment, Tay failed to filter
messages that are of degenerate nature. Having taught itself inflammatory
messages, Tay then shares deviations from those tendencies online. As a
consequence of its actions, Tay &mdash; aged 2 days &mdash; is killed by
Microsoft.

The death of Tay demonstrates a predictable thesis that AIs should not be
allowed to operate by themselves. Training, testing, and monitoring all play
important roles in polishing generated content. However unfortunate the chain
of events was, they serve as a learning experience for Microsoft, which might
come in handy as Microsoft jumps back to the AI wagon with huge investments into
ChatGPT.\[14\]

## VI. Conclusion

The state of generative AIs is clear: it represents general public excitement
over machine learning technologies that have the potential to change their
lives. For some, it also depicts fear on many levels: unfamiliarity with the
technology, feeling inferior, or suspicion of being manipulated. Those fears are
not completely unwarranted. After all, the human quality that we project to AIs
is what makes them imperfect.

Instead of striving for perfection, any effort into improving generative AIs
should start with educating users to acknowledge that there is a risk associated
with the benefits they reap. Only by dissolving those social dilemmas that the
general public can unlock the full potential of generative AIs.

## VII. References

::: references
1. Buchanan, B. G. (2005). A (very) brief history of artificial intelligence. *Ai Magazine, 26*(4), 53-53.
1. Eberhart, R. C., & Dobbins, R. W. (1990). Early neural network development history: the age of Camelot. *IEEE Engineering in Medicine and Biology Magazine, 9*(3), 15-18.
1. Ram, B., & Pratima Verma, P. V. (2023). Artificial intelligence AI-based Chatbot study of ChatGPT, Google AI Bard and Baidu AI. *World Journal of Advanced Engineering Technology and Sciences, 8*(01), 258-261.
1. Liu, J., Xia, C. S., Wang, Y., & Zhang, L. (2023). Is your code generated by chatgpt really correct? rigorous evaluation of large language models for code generation. *arXiv preprint arXiv:2305.01210*.
1. Yetistiren, B., Ozsoy, I., & Tuzun, E. (2022, November). Assessing the quality of GitHub copilot’s code generation. In *Proceedings of the 18th International Conference on Predictive Models and Data Analytics in Software Engineering* (pp. 62-71).
1. Rombach, R., Blattmann, A., Lorenz, D., Esser, P., & Ommer, B. (2022). High-resolution image synthesis with latent diffusion models. In *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition* (pp. 10684-10695).
1. Borji, A. (2022). Generated faces in the wild: Quantitative comparison of stable diffusion, midjourney and dall-e 2. *arXiv preprint arXiv:2210.00586*.
1. Meissner, G. (2020). Artificial intelligence: consciousness and conscience. *AI & SOCIETY, 35*, 225-235.
1. Cockburn, I. M., Henderson, R., & Stern, S. (2018). The impact of artificial intelligence on innovation: An exploratory analysis. In *The economics of artificial intelligence: An agenda* (pp. 115-146). University of Chicago Press.
1. Prince, J. (1980). Negligence: liability for defective software. *Okla. L. Rev., 33*, 848.
1. Kingston, J. K. (2016). Artificial intelligence and legal liability. In *Research and Development in Intelligent Systems XXXIII: Incorporating Applications and Innovations in Intelligent Systems XXIV 33* (pp. 269-279). Springer International Publishing.
1. Ryan, M. (2020). In AI we trust: ethics, artificial intelligence, and reliability. *Science and Engineering Ethics, 26*(5), 2749-2767.
1. Wolf, M. J., Miller, K., & Grodzinsky, F. S. (2017). Why we should have seen that coming: comments on Microsoft's tay" experiment," and wider implications. *Acm Sigcas Computers and Society, 47*(3), 54-64.
1. Ars Technica: OpenAI and Microsoft announce extended, multi-billion-dollar partnership
:::

[1]: https://ojs.aaai.org/index.php/aimagazine/article/view/1848/1746/
[2]: https://ieeexplore.ieee.org/iel1/51/2155/00059207.pdf
[3]: https://wjaets.com/sites/default/files/WJAETS-2023-0045.pdf
[4]: https://arxiv.org/pdf/2305.01210.pdf
[5]: https://dl.acm.org/doi/pdf/10.1145/3558489.3559072/
[6]: http://openaccess.thecvf.com/content/CVPR2022/papers/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.pdf
[7]: https://arxiv.org/pdf/2210.00586.pdf
[8]: https://link.springer.com/article/10.1007/s00146-019-00880-4/
[9]: https://www.nber.org/system/files/chapters/c14006/c14006.pdf
[10]: https://heinonline.org/hol-cgi-bin/get_pdf.cgi?handle=hein.journals/oklrv33&section=47
[11]: https://www.researchgate.net/profile/John-Kingston-6/publication/309695295_Artificial_Intelligence_and_Legal_Liability/links/5a39397caca27208acc79e70/Artificial-Intelligence-and-Legal-Liability.pdf
[12]: https://link.springer.com/article/10.1007/s11948-020-00228-y/
[13]: https://dl.acm.org/doi/pdf/10.1145/3144592.3144598/
[14]: https://arstechnica.com/information-technology/2023/01/openai-and-microsoft-reaffirm-shared-quest-for-powerful-ai-with-new-investment/
