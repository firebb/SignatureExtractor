# SignatureExtractor

This is simple tool to extract the signature page from pdf files generated from word. It depends on Apache pdfbox and commons CLI. It works through extracting word from the pdf, so this would not work on scanned pdfs. Currently it is a command line tool so no gui is support. No plan to add gui either.

## Dependency and PreInstall

This tool need java runtime. Please follow the instructions to install java first.
https://java.com/en/download/mac_download.jsp

## Command Line Hint
Head into System Preferences and select Keyboard > Shortcuts > Services. Find "New Terminal at Folder" in the settings and click the box. 

## Usage
1. Download the SigExtractor.jar file. It should be in the Download directory.
2. command + space to use spotlight search, type terminal and enter.
3. Type `cd Downloads/`
4. Type `ls`, you should be able to see the SigExtractor.jar file.
5. To run the jar file, type `java -jar SigExtractor.jar -h` and you would see the help information.

## Example                  
1. Put the pdf you want to extract in the same directory as the jar file. Say example.pdf
2. Use Terminal to enter the directory.
3. Type `java -jar SigExtractor.jar -i example.pdf`
4. By default, the tool would extract all pdf pages with the text "signature page" and store them as SignaturePage[PageNum].pdf

Basically, the tool supports the following options:
-k searchkey: the word to find the pages needed to be extracted.
-p 1,2,3: directly extract given pages numbers.
-o outputname: define the output name.

## More
This is a README file for people who don't uses terminal a lot, like lawyers. As I'm not get paid, only limited tech support would be provided.

## Acknowledgements
Little tool for a better life for Jazzy. - ~ -
