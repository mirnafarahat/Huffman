# Huffman

# Huffman Coding Implementation in Java

This project demonstrates the implementation of Huffman coding, a lossless data compression algorithm, in Java. Huffman coding is widely used for data compression, where more frequent characters are represented with shorter codes, optimizing the storage or transmission of data.

## Features

- The `Node` class defines individual nodes for the Huffman tree, storing character, frequency, and references to left and right nodes.
- The `PriorityQueue` class implements a priority queue used in building the Huffman tree.
- The `TreeHuffman` class represents the Huffman tree, providing methods to display its structure and obtain character-code mappings.
- The `CodeHuffman` class manages encoding and decoding using the Huffman tree, along with building and displaying the Huffman tree and code table.

## Usage

The project demonstrates encoding and decoding using Huffman coding. The `CodeHuffman` class provides methods to encode and decode messages based on a Huffman tree generated from input messages.

Here's a simple example of usage:

```java
// Create a CodeHuffman instance with the input message
CodeHuffman huffman = new CodeHuffman("example message");

// Build the Huffman tree
huffman.TreeBuild();

// Display the Huffman tree structure
huffman.TreeDisplay();

// Encode a message using the Huffman tree
String encodedMessage = huffman.encode("example");

// Decode an encoded message using the Huffman tree
String decodedMessage = huffman.decode(encodedMessage);

System.out.println("Encoded message: " + encodedMessage);
System.out.println("Decoded message: " + decodedMessage);

Feel free to explore the code and experiment with different messages to encode and decode. Huffman coding is a fundamental concept in data compression and provides a way to efficiently represent data using variable-length codes.

For more details, refer to the source code files provided in the repository.
