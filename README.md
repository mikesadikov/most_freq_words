
## Multi-threaded counting of the most frequent words

Multi-threaded C++ program for counting the most frequent words in text files.

Parallelization strategy: 
each thread has its own dictionary for counting the occurrence of words, after the completion of the threads, these dictionaries merge together. 

## build instructions:

To build the project, run the following commands:

```
mkdir build && cd build
cmake ..
cmake --build .
```

##  Usage example:

```
topk_words number_of_threads(1..10), topk_words(3..10), [FILES...]
```

number_of_threads - number of threads :-) 
topk_words - number of displayed words,
[FILES...] - list of processed text files.

For example:
```
topk_words 5 10 64317-0.txt pg1777.txt
```
