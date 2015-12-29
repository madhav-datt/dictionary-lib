# dictionary-lib
C language Dictionary Library designed to use the English dictionary in Trie data structures for fast spell-checking.
This library can be used to load a dictionary file into memory and spellcheck over 1 million words in close to 1 second.

## Library Contents and Functions

* `LENGTH` - Assumed maximum word length in dictionary
* `bool check (const char* word)` - Checks if `word` is present in the dictionary - ie. is correctly spelled. Returns true if word is in dictionary else false.
* `bool load (const char* dictionary)` - Loads dictionary into memory.  Returns true if successful else false.
* `unsigned int size (void)` - Returns number of words in dictionary if loaded else 0 if not yet loaded.
* `bool unload (void)` - Unloads dictionary from memory.  Returns true if successful else false.

## Dictionary File 

The dictionary file must be loaded to memory using the `load (dictionary)` function. The dictionary must be in a .txt format, with each word in a new line. The `Dictionary.txt` file included with the release contains 358232 words and can be used.

## Using the library

### Downloading the library

    $ wget https://github.com/madhav-datt/dictionary-lib/archive/dictionary-lib.v2.0.zip
    $ unzip dictionary-lib.v2.0.zip
    $ rm -f dictionary-lib.v2.0.zip

### Using the library in a program

Include the following header file in your program:

    #include "/Downloads/dictionary-lib.v2.0/lib/dictionary.h"
