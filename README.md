# CodeChallenge
Use:
Download and install CLI.py to run main function. 

Sample inputs:


python3 CLI.py <URL> 

python3 CLI.py <URL> -c nThreads
  
  
CLI.py has two main functions that handle file downloads through the command line. For the args_thread_handler() function it uses argparse to implement the CLI and any arguments that required or optional to be parsed. It requires the user to input an URL to be downloaded with the optional argument -c nThreads that specify the number of threads to be used during download. 

It uses the threading library to handle  any extra threading processes, also allowing for multiple URLS to be concurrently downloaded for future scaling. For the downloader function it reads the file that is being downloaded in multiple chunks (in bytes) as to not read the entire file into memory at once. It uses the tqdm library to implement a progress bar for files that are downloading
and specifies completion at the end. Files that are unable to be downloaded are given an error message to the user. 
