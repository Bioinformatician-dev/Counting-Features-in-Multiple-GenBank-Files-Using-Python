
# Counting Features in Multiple GenBank Files Using Python

In this task, we aim to create a Python script that can parse multiple GenBank files and count the various biological features present in each file. GenBank files are widely used in bioinformatics to store nucleotide sequences and their annotations. By counting the features, we can gain insights into the biological data contained within these files.






## Authors

- [@Salma](https://www.github.com/Bioinformatician-dev)


## Explanation


The provided Python script utilizes the Biopython library to parse GenBank files and count the features within them. Here’s a breakdown of the code:

Imports:

SeqIO from the Bio module is used for reading GenBank files.
os is used to interact with the file system.
defaultdict from the collections module allows us to create a dictionary that defaults to another dictionary, which is useful for counting.
Function Definition:

The function count_features_in_genbank_files(directory) takes a directory path as an argument. This directory should contain the GenBank files.
Iterating Through Files:

The script iterates through all files in the specified directory. It checks if the file has a .gb or .gbk extension, indicating that it is a GenBank file.
Parsing GenBank Files:

For each GenBank file, it opens the file and uses SeqIO.parse() to read the records. Each record represents a sequence entry in the GenBank file.
Counting Features:

The script iterates through the features of each record. It retrieves the feature type and increments the count in the feature_counts dictionary.
Returning Results:

After processing all files, the function returns a nested dictionary containing the counts of each feature type for each file.
Example Usage:

The script includes an example usage section where you can specify the path to your GenBank files. It then prints the feature counts for each file in a readable format.
