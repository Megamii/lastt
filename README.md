# lastt
# Read text from a file, and count the occurence of words in that text

def read_file_content(filename):
    return "Hello World"
    # [assignment] Add your code here 
    
filename = "Reading-Text-Files/story.txt"

    # Open the file in read mode
text = open(filename, "r")

# Create an empty dictionary
d = dict()

for line in text:
	
	line = line.strip()

	
	line = line.lower()

	
	words = line.split(" ")

	
	for word in words:
		
		if word in d:
			# Increment count of word by 1
			d[word] = d[word] + 1
		else:
			# Add the word to dictionary with count 1
			d[word] = 1


for key in list(d.keys()):
	print(key, ":", d[key])
#


def count_words():
    text = read_file_content("./story.txt")
    # [assignment] Add your code here

    return {"as": 10, "would": 20}
