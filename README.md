# apologia

A bilingual (French / English) evangelical-Protestant apologetics **field reference**,
typeset with the [texish](https://github.com/edadma/texish) document engine.

The document is a deck of one-page "cards," each answering a common question or objection
with a short answer, a few key points, and the scripture printed in full so it can be read
straight from the page. It is laid out for a small half-letter booklet (5.5 × 8.5 in): the
French take of each card sits on the left (verso) page and the matching English take on the
right (recto), so the two languages always face each other. A trilingual cover (Greek title
*Ἀπολογία* with French and English subtitles) and separate French and English tables of
contents open the book; the cover carries the full date as a version stamp.

Scripture is quoted from public-domain translations — **Louis Segond 1910** in French and the
**Berean Standard Bible** in English.

## Contents

| Section | Cards |
|---|---|
| Sharing the Gospel | Opening questions · The good news · Leading to faith |
| The Existence of God | Evidence and science |
| The Reliability of the Bible | Contradictions · Reliable transmission |
| Jesus | Just a good teacher · A legend |
| Suffering and Evil | Why suffering |
| Other Religions | All roads to God |
| Science and Faith | Evolution |
| Morality | Good without God |
| The Church and Me | Hypocrites · I'm a good person |

## Building

The source is a single texish document, `apologia.texish`. Render it to PDF from a texish
checkout (fonts load relative to the working directory):

```sh
cd /path/to/texish
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia.texish
```

This writes `apologia.pdf` beside the source. The rendered PDF is not tracked in this
repository.
