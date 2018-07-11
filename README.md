*********************************  README TEXT  *********************************

Object orientated software development: Final Assignment

Justin Kelly

The application is set up with the following classes:
	-Runner class as required.
	-Menu class
	-Parse class
	-FourSquareCipher class

Comments have been added to the code to explain the code

The application can be run by compilling the application first and then entering 
	java.ie.gmit.dip.Runner
into the command prompt.

After starting the appllication the user will be brought to the menu screen, where there will be four options available

Note: A try catch block has been added to catch the "number format exception" and to print out an appropriate message to the user. No stack trace has been added as these are generally FRIGHTENING for users.

*****The user must enter a keyword first before beginning with the encryption or decryption process. Otherwise they will get a nullpointer exception.// comments in the code show why this occurs*******
This could have been avoided by assigning the default matrix to the newArray variable in the menu class but this duplicate code was not the correct solution i thought.

1) Create key(s)
The user is able to enter two keywords. One at a time. 
The first keyword(s) entered will  have all whitespace, special characters, j's and duplicate letters removed and the remaining characters will be placed in order into the top right part of the four square cipher (or matrix as the instance variable is called) followed by any remaining letters of the alphabet if they have not been used in the keyword(s).
The same will happen for the second keyword but it will be entered into the bottom left portion  of the four square cipher.

2) Encrypt file or url
The user can now choose to enter a file name including file extension or url in the command line and this file or url will then be encrypted line by line ignoring the blank lines in a document(for example the blank lines in the war and peace document)
A url such as https://www.google.com/ can be entered and the application will encrypt the source code of the site. ( HTML and Javascript)
The encrypted file will then be output locally to the file: encrypted.txt.
The encrypting process will be based on the last keywords that have been entered so if you want to encrypt a file it would make sense to add the keywords first yourself so you will then in turn be able to decrypt the file as required.

3) Decypt file or url
The user can now choose to enter a file name including file extension or url in the command line and this file or url will then be decrypted line by line ignoring the blank lines in a document.
The decrypted file will then be output locally to the file: decrypted.txt.
The decrypting process will be based on the last keywords that have been entered so if you want to decrypt a file you need to have entered the same keys that have been used in the encryption process.

4) Quit the application
The application terminates.

