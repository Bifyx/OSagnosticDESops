
# Installation of SageMath by Bianca Okeke

### The following are the steps I took in installing SageMath

1. I use a Windows system so I clicked on this website [https://github.com/datascience-intro/how2_WindowsOS10-\_2SageMath-2021](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021)
2. Downloaded the sage source code from this website.[https://github.com/datascience-intro/how2_WindowsOS10-\_2SageMath-2021](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021)
3. Using the above link, I used the information on: Ubuntu on Windows Subsystem for Linux (WSL) prerequisite installation
4. I enabled hardware-assisted virtualization in my system. Mine is UEFI.
5. Ran Powershell as an administrator and installed Windows Subsystem for Linux **wsl --install**.
6. Immediately, the Ubuntu downloaded and the system asked for a reboot.
7. After the reboot, Ubuntu couldn't install and I had to open *Turn Windows Features on or off* and ticked the *Windows Subsystem for Linux*.
8. I downloaded Ubuntu 20.04 from the Microsoft store.
9. Then followed the steps to upgrade to Ubuntu 20.10. I didn't have the'update-manager-core package installed'. I used the information from this website, [https://www.linuxbabe.com/ubuntu/upgrade-ubuntu-20-04-to-ubuntu-20-10](https://www.linuxbabe.com/ubuntu/upgrade-ubuntu-20-04-to-ubuntu-20-10).
10. At the point of  *'sudo do-release-upgrade'*, I kept getting error messages. I used **'sudo apt-get purge snapd'** and  **'sudo apt-get autoremove'** repectively before reusing **'sudo do-release-upgrade'** and upgrade began which took hours.
11. After installing the required prerequisites, I started SageMath installation.
12. It took me a while to figure out what step one  of the SageMath installation guide meant, I had to watch YouTube videos. I deleted the first download I did from this website, [https://github.com/datascience-intro/how2_WindowsOS10-\_2SageMath-2021](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021), and re-downloaded in the Ubuntu terminaal. I also created a directory to store the SageMath.
13. I got an error so many times using **'make'** and **'make -j2'** so I decided to search online. After so many failed attempts, finally found the method below which worked. I also added modifications where necessary.
    * **'cd sage'**
    * **'make configure'**
    * **'./configure --with-python=3'**
    * **'MAKE="make -j2" make'**

14. It started installation which took more than 14 hours.

**It took me over 48 hours to complete the steps as I had errors and made lots of mistakes.**






# OSagnosticDESops

This is a repository for instructions on how to do Operating System Agnostic Data Engineering Science Operations, especially for students of Mathematics, Computer Science, Statistics, Data Science and Data Engineering.

## Problem 0, Individual Assignment 3

Please do the following STEPS to document your installation of SageMath on your laptop's and/or desktop's operating system(s):

1. STEP 0: Get a Github Account at https:/github.com if you do not already have one and install git on your laptop by following this [Quickstart](https://docs.github.com/en/get-started/quickstart) with these two minimal steps:
    - [Hello World](https://docs.github.com/en/get-started/quickstart/hello-world)
    - [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
2. STEP 1: fork **this** GitHub repository: [https://github.com/datascience-intro/OSagnosticDESops](https://github.com/datascience-intro/OSagnosticDESops) 
    - the easiest way is to login to your GitHUb account and go to the above URL, 
    - click the 'fork' button from the web browser [as shown here](images/fork00.png),
    - choose your GitHub username where you want the fork of OSagnosticDESops repository to go to [as shown here](images/fork01.png),
    - now you should be able to see your fork of the repository at `https://github.com/yourGitHubUsername/OSagnosticDESops/` [as shown here](images/fork02.png),
    - go to `Code` and chose one of the methods (SSH is recommended; HTTPS or CLI are also ok; see [connect with SSH](https://docs.github.com/en/enterprise-server@3.0/authentication/connecting-to-github-with-ssh) for the setup instructions) [as shown here](images/fork03.png),
    - finally you can go into the appropriate directory in your local machine (laptop/desktop) and clone your fork of the repository [as shown here](images/fork04_cloneYourForkLocally.png),
    - you can stay up to date with the upstream [https://github.com/datascience-intro/OSagnosticDESops](https://github.com/datascience-intro/OSagnosticDESops) [as showh here](images/fork05_fetchAndMetgeUpstream.png) and commit and push your own changes by taking a brief tour of [git](https://en.wikipedia.org/wiki/Git) and completing other steps in [Quickstart](https://docs.github.com/en/get-started/quickstart).
3. STEP 2: You main task is to document the steps you took to install SageMath the easy way from binaries or the harder way from source on your local machine, by following the guidelines in:
    - [https://github.com/datascience-intro/how2_MacOSX_2SageMath-2021](https://github.com/datascience-intro/how2_MacOSX_2SageMath-2021)
    - [https://github.com/datascience-intro/how2_WindowsOS10-\_2SageMath-2021](https://github.com/datascience-intro/how2_WindowsOS10-_2SageMath-2021)
    - You may either document using markdown by editing this `README.md` file in your fork of this repository by simply writing down the steps you took to install SageMath
    - Or give a URL to another repository that documents your installation steps in detail
    - The main expectation is that you should be able to install SageMath on your local machine a lot faster by following the instructions you have given
 
Further instructions, if needed, will follow shortly after the computer labs in Angstrom are tested. Please discuss in threads at the course instructure page so you can learn from one another.




