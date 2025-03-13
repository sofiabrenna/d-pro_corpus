# D-Pro Corpus
D-Pro (Dialogue-Proactivity) is a corpus of 151 human-human task-oriented dialogues annotated for proactivity.
The dialogues are primarily in Italian and originate from five different source corpora, comprising a total of 2,855 turns and 6,028 utterances.

## Defining Proactivity
Proactivity is a pragmatic collaborative phenomenon that can be regarded as the ability to show initiative by providing unsolicited yet relevant contributions to the dialogue’s topics and goals. We say that an utterance in the context of a task-oriented dialogue is considered as proactive when one of the participants, either Agent or Client:
  1. does not act merely in response to the requests the other participant has made, so the behaviour is self-prompted and not simply reactive;
  2. has a long-term, goal-directed behaviour that predicts future states and needs, so the behaviour is somehow effective for the achievement of the dialogue goal.

### Source Corpora
The D-Pro corpus integrates dialogues from the following datasets:
- Italian NESPOLE! Corpus (Mana et al., 2003): A collection of Italian role-playing phone call dialogues from the multilingual and multimodal NESPOLE! project. The   conversations involve a tourist calling a travel operator to arrange a vacation in the Trentino region of Italy.
  
  Link: https://aclanthology.org/www.mt-archive.info/LREC-2002-Costantini.pdf
- Italian WhatsApp Corpus (Hewett, 2017): A dataset of two-party and multi-party chat dialogues in Italian, sourced from WhatsApp conversations of users based in     Germany and Italy. Task-oriented dialogues were manually extracted from the conversations. Due to participants’ code-mixing and code-switching, minor parts of      the corpus are in English and a few utterances are in German.
  
  Link: https://www.uni-potsdam.de/en/la-bank/digital-communication/italian-whatsapp-corpus
- Italian Ubuntu Chat Corpus (Lowe et al., 2015): A multilingual dataset of multi-party IRC chat logs from Ubuntu’s technical support channel for Italian users.      The corpus includes dialogues where users, identified by nicknames, seek assistance for Linux-based Ubuntu issues.

  Link: https://daviduthus.org/UCC/
- MultiWOZ 2.2 Corpus (Zang et al., 2020): An updated version of the MultiWOZ dataset (Budzianowski et al., 2018), containing multi-domain, Wizard-of-Oz-style        scripted dialogues in English. Conversations simulate interactions between a tourist client (User) and an information center agent (System).

  Link: https://github.com/budzianowski/multiwoz/tree/master/data/MultiWOZ_2.2
- JILDA Corpus (Sucameli et al., 2021): An Italian dataset of human-human dialogues in the job search and recruitment domain. Conversations, collected via role-      playing, feature a job-seeking Client interacting with an Agent who assists in the search process.

  Link: https://github.com/IreneSucameli/JILDA

## Annotation Schema
### Proactivity Annotation
Each utterance is labeled as either:
- proactive
- not_proactive

A dialogue turn is considered proactive if it contains at least one proactive utterance.

### Dialogue Act Annotation
Each proactive utterance is categorized into one of the following Dialogue Acts based on Bunt’s (2010) ISO taxonomy:
- inform
- offer
- suggest
- request
- instruct.

### Goal Failure Annotation
Utterances indicating failure to achieve a dialogue goal are marked with a "fail" tag. These goal failure situations are particularly interesting because they often require proactive responses for repair: this annotation helps us better understand the link between goal failure and proactive behaviour.
 
### Turn Adjacency Annotation
To capture the conversational context of proactivity, we analyze the relationship between a proactive utterance and its preceding turn. If the previous turn provides sufficient context to justify proactivity, the proactive utterance is marked with the "adjacent" tag. If longer dependencies can be found with the previous context, the proactive utterance is non adjacent.

## D-Pro WhatsApp Distribution
Access to D-Pro_WHATSAPP subcorpus can be requested by contacting the owners of the The Italian Whatsapp Corpus at langage@uni-potsdam.de (https://www.uni-potsdam.de/en/la-bank/digital-communication/italian-whatsapp-corpus).

## Contributors
- Sofia Brenna (Free University of Bozen-Bolzano, FBK - Fondazione Bruno Kessler)
- Elisabetta Jezek (Univerity of Pavia)
- Bernardo Magnini (FBK - Fondazione Bruno Kessler)

## Cite
If you find this corpus useful, please cite the following article:

```bibtex
@article{brenna2025investigating,
  title={Investigating Proactivity in Task-Oriented Dialogues},
  author={Brenna, Sofia and Jezek, Elisabetta, and Magnini, Bernardo},
  journal={Dialogue \& Discourse},
  volume={16},
  number={1},
  pages={31--66},
  year={2025}
}
```
S. Brenna, E. Jezek, B. Magnini. Investigating Proactivity in Task-Oriented Dialogues. Dialogue & Discourse 16(1) 31-66. To be published online 03/2025.
