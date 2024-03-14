这个词库是我多年前收集整理的，已经忘记了原始出处，是多个词库的并集。
其中`base_AND_large.txt`经过了程序和人工审核，其他词库只进行了程序审核。其中存在的问题是，收录了一些不是词的词，不是短语的短语。去除这部分比较困难。

现在依据[mozillazg](https://github.com/mozillazg/phrase-pinyin-data)中的`large_pinyin.txt`，再次进行形式上的审阅。

`base_AND_large.txt`是`large_pinyin.txt`与我的核心词库的交集，经过了人工审核。其词频是真实词频。

`expand_corpus_AND_large.txt`是`large_pinyin.txt`与我的扩充词库的交集，只进行了程序审核。
其拼音直接使用了`large_pinyin.txt`中的拼音。
其词频是被其他词库收录的统计，不是真实词频。

`other_large.txt`是`large_pinyin.txt`不与我的词库交集的集合。其词频设置为1。

`base_AND_large.txt`+`expand_corpus_AND_large.txt`+`other_large.txt`就是原`large_pinyin.txt`中收录的词。

现对`base_AND_large.txt`中的拼音进行审核，校订其中大约一千多个词的拼音。