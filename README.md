# Integrated-Russian-Sentiment-Lexicons
This dataset is an integrated collection derived from four open-source Russian sentiment lexicons: RuSentiLex, Karta Slov, PolSentiLex (Linis Crowd project), and the KFU Sentiment Dictionary. 

- **The Sentiment Core list** includes 8,588 non-neutral entries whose sentiment annotations are consistent across at least three sources. 

- **The Sentiment Integrated list** contains 20,272 non-neutral entries with no conflicts of opposite sentiment polarity.

## 🔎 Source Lexicons Description

The integration is based on the following open sentiment lexicons:

### RuSentiLex (≈16,000 entries)
A lexicon from tonal dictionaries enriched with data from Twitter and news texts.
Entries are annotated for sentiment polarity (positive, negative, neutral, mixed) and subjectivity (fact, opinion, feeling). Polarity may vary across different synsets in the Russian thesaurus RuThes (e.g., нежный: negative “fragile / too weak” vs. positive “gentle / affectionate”).
(Loukachevitch & Levchik, 2016)

### Karta Slov Sentiment Lexicon (≈46,000 entries)
Crowd-sourced sentiment annotations obtained via the “Karta Slov” lexical resource.
Words are labeled for polarity (positive, negative, neutral) and intensity on a scale from −1 to 1
(Kulagin, 2021)

### PolSentiLex (7,546 entries)
A sentiment lexicon created via crowd-sourced polarity judgments in social and political contexts from blogs and social media.
Sentiment values range from −2 to 2
(Koltsova et al., 2016)

### KFU Sentiment Lexicon (≈25,000 entries)
A hybrid sentiment lexicon developed at Kazan Federal University.
Polarity for 1,000 words was annotated via crowdsourcing, while the remaining entries were extrapolated using a BERT-based model trained on news texts and Russian Wikipedia.
Sentiment is represented as a continuous score from 0 to 1
(Solovyev et al., 2022)

These four lexicons show very low overlap: for negatively valenced words, only 717 entries (4%) appear in all four sources. Similarly, for positively valenced words, the intersection consists of 305 entries (3.4%).

## 🧩 Integrated List

**Sentiment Core List** — a strict intersection of lexicons, containing 8,588 non-neutral words whose sentiment polarity is consistent across at least three sources.

**Sentiment Integrated List** — a maximally inclusive collection of 20,272 non-neutral words without any conflicts in opposite polarity.

Both the Core and Integrated collections were expanded with adverbs derived from sentiment-bearing adjectives, provided that the adverb form appears in a Russian frequency dictionary (e.g., абсурдный – абсурдно, жестокий – жестоко, etc.).

The adverbs inherit the polarity of the corresponding adjective:

Core List: +818 adverbs
Integrated List: +956 adverbs

## ⚖️ Licensing and Attribution

This repository contains transformed and integrated versions of existing open lexicons. Each source lexicon remains the intellectual property of its original authors and is redistributed under its original license.

Please cite the original resources when using the data.

**Карта слов**: 

https://github.com/dkulagin/kartaslov

Кулагин Д. И. Открытый тональный словарь русского языка «КартаСловСент». Компьютерная лингвистика и интеллектуальные технологии: По материалам ежегодной Международной конференции «Диалог». Вып. 20. М.: Изд-во РГГУ, 2021, с. 1106–1119.

**RuSentiLex**:

https://www.labinform.ru/pub/rusentilex/index.htm

Loukachevitch N., Levchik A., 2016. Creating a General Russian Sentiment Lexicon. In Proceedings of Language Resources and Evaluation Conference LREC-2016. 

**PolSentiLex**:

https://github.com/hse-scila/PolSentiLex

Koltsova, O., & Alexeeva, S. (2015). Linis-crowd.org: A lexical resource for Russian sentiment analysis of social media. Computational Linguis- Tics and Computantional Ontologies: Proceedings of the XVIII Joint Conference “Internet and Modern Society (IMS-2015), 25–34. 

**Sentiment Dictionary KFU**:

Solovyev V., Islamov M., Bayrasheva V. Dictionary with the Evaluation of Positivity/Negativity Degree of the Russian Words. In: Prasanna S.R.M., Karpov A., Samudravijaya K., Agrawal S.S. (eds) Speech and Computer. SPECOM 2022. Lecture Notes in Computer Science, vol 13721. Springer, Cham, 2022. https://doi.org/10.1007/978-3-031-20980-2_55

