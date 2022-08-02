# Data Compression and Decompression using Huffman Coding Technique

## Overview

A desktop application built with Java Swing (JLabel, JPanel, JScrollPane, JTextArea, JButton, JFileChooser) using the concepts of Priority Queue, Hash Map, Map and Comparator which focuses mainly on compressing and decompressing text data. 
It takes an input from the text box or from a file that contains data in the form of text and compresses it using the Huffman coding technique. 
It also displays the Huffman codes and the decompressed text.

## Data Compression

Data compression involves encoding the information in a file in such a way that it takes up less space. It basically aims to make files smaller.

Smaller files 
1. Use less storage, resulting in cost savings.
2. Can be transmitted faster, decreasing access time or, alternatively, allowing the same access time with a lower and cheaper bandwidth.
3. Can be processed faster sequentially.

Many techniques are available for compressing data, one of them is by assigning variable-length codes.

## Assigning Variable-Length Codes

Variable-length codes are based on the principle that some values occur more frequently than others, so the codes for those values should take the least amount of space. It is a form of redundancy reduction.

Morse code is the oldest and common scheme of the variable-length codes. In this scheme we use two different symbols: a dot (.) and a dash (-) to encode the characters. We determine the most frequently occurring characters and assign a single dash or dot to it. The other less frequently occurring characters are represented with two or more symbols.

Morse code can be implemented using a table lookup, where the table never changes. Since many sets of data values do not exhibit a predictable frequency distribution, more modern variable-length coding techniques dynamically build the tables that describe the encoding scheme. One of these is Huffman code.

## Huffman Code

Huffman code determines the probabilities of each value occurring in the data set and builds a binary tree in which the search path for each value represents the code for that value. Most frequently occurring values are given shorter search paths in the tree. This tree is then converted into a table, that can be used to encode and decode the data.

## Application Screenshots
### 1. Home screen

![Screenshot (1)](https://user-images.githubusercontent.com/74103829/181489631-39fe64d8-98ba-4d35-85aa-92e93168735d.png)

### 2. User input in the form of text

![Screenshot (2)](https://user-images.githubusercontent.com/74103829/181493206-45fda3f6-6d05-4866-a946-6ae51130668a.png)

### 3. Output in the form of Huffman codes, compressed and decompressed text

![Screenshot (3)](https://user-images.githubusercontent.com/74103829/181493581-628759cc-7252-4b49-890c-d2f59b85f697.png)

### 4. User input in the form of file stored in the local system

![Screenshot (4)](https://user-images.githubusercontent.com/74103829/181494439-f2546c13-3bef-48ce-bdbb-c767d6d10a18.png)

### 5. Output in the form of Huffman codes, compressed and decompressed text

![Screenshot (5)](https://user-images.githubusercontent.com/74103829/181494655-1b6103df-eced-4c29-a2dd-35ad8a31566d.png)
