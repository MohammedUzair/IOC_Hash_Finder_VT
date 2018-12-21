# IOC_Hash_Finder_VT
The power shell script reads multiple MD5, SHA1 or SHA256 hash values line by line from a file and search for it's corresponding hash values with the help of VirusTotal Database. 
Before you run the script, please:
    1.  SignUp in VirusTotal.com to get th API_KEY, which is mandatory to send any requests to VirusTotal.
    2.  Create the following folder: "C:\VT_IOC_Hash_Matcher"
    3.  Rename your input file (with hash values) to "Input.txt" 
    4.  Copy the input file to the folder: "C:\VT_IOC_Hash_Matcher"
    5.  Please make sure you have write permissions for the folder ""C:\VT_IOC_Hash_Matcher"
    6.  Run the script, you may find two output files inside the folder "C:\VT_IOC_Hash_Matcher" with names:
            a. Output_Matched_Hashes.csv (Contains all matched hash values and their corresponding hashes")
            b. Output_No_Match_Hashes.txt (Contains all hash values which were not a match in VirusTotal)

Please note that the VirusTotal limits the request to the website using an API Key as 4 requests per minute. Hence, to have 12 number of hashes searched, the script requires 12/4=3 minutes to complete. In case you have a Premium API Key bought from VirusTotal, which comes with no restrictions on the number of requests to VirusTotal.com, feel free to get rid of the code which makes the script wait for 16 seconds after every request. 

Queries:
https://www.linkedin.com/in/iamshahrukh/


