# code_failed
from nltk.corpus.reader import PlaintextCorpusReader
source_dir = "爬蟲"
pcr = PlaintextCorpusReader(root=source_dir, fileids="M.1632715576.A.195.html.txt")

from nltk.probability import FreqDist
fd = FreqDist(samples=pcr.words())
print(fd.most_common(n=100))
