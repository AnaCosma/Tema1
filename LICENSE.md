with open('listofwords.txt') as f: # note: 'r' is the default mode
    lines = f.readlines() # also: using `with` is good practice
for line in lines:
    word = line.strip()
    wordsorted = ''.join(sorted(line))
    for word in lines:
        if word == ''.join(sorted(word)):
            print word
