# command-similarity-measurement

Process invocations happen with almost every activity on a computer. To distinguish user input
and potentially malicious activities, we need to better understand program invocations caused
by commands. To achieve this, one must understand commands’ objectives, possible parameters,
and valid syntax. In this work, we collected commands’ data by scrapping commands’ manual
pages, including command description, syntax, and parameters. Then, we measured command
similarity using two of these – description and parameters – based on commands’ natural language
documentation. We used Term Frequency-Inverse Document Frequency (TFIDF) of a word to
compare the commands, followed by measuring cosine similarity to find a similarity of commands’
description. For parameters, after measuring TFIDF and cosine similarity, the Hungarian method
is applied to solve the assignment of different parameters’ combinations. Finally, commands are
clustered based on their similarity scores. The results show that these methods have efficiently
clustered the commands in smaller groups (commands with aliases or close counterparts), and
in a bigger group (commands belonging to a larger set of related commands, e.g., bitsadmin for
Windows and systemd for Linux). To validate the clustering results, we applied topic modeling on
the commands’ data, which confirms that 84% of the Windows commands and 98% ofthe Linux
commands are clustered correctly.


# Cite as:
Hussain, Z., Nurminen, J. K., Mikkonen, T. & Kowiel, M. “Command Similarity Measurement Using NLP” 10th Symposium on Languages, Applications and Technologies, 2021.
