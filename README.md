# CS410-CourseProject-Team-AEJ

## Project Topic: 
Perform sentiment analysis on Twitter tweets for a given brand to help companies gain insights on
their brand or on product(s).

## Project Files:
1. **Project Final Report**: Final_Report/CS410_Final_Project_Report_Team-AEJ.pdf
2. **Project Presentation**: Final_Report/CS410_Project_Presentation_Team-AEJ.pptx
3. **Project Demo/Video**: https://mediaspace.illinois.edu/media/t/1_tujkacb5
4. **Project Proposal File**: Project_Proposal_Progress_Docs/CS410_Project_Proposal_Team-AEJ.pdf
5. **Project Progress Report**: Project_Proposal_Progress_Docs/CS410_Project_Progress_Report_Team-AEJ.pdf

[Install on Windows | Docker Documentation]: https://docs.docker.com/desktop/install/windows-install/
[Install on Mac | Docker Documentation]: https://docs.docker.com/desktop/install/mac-install/

## Software Usage Details
Outlined below are the installation and set up instructions for our software.
### Install the Docker Image
* Please install **Docker** in your machine:
  * Use this link if you are running the software on Windows: [Install on Windows | Docker Documentation]
  * Use this link for Mac installation: [Install on Mac | Docker Documentation]
* Once installed, start Docker Engine in your machine.
<p align="center">
  <img src="./img assets/docker 1.png" alt="Docker Install ribbon" width="350">
  <img src="./img assets/docker2.jpg" alt="Docker Desktop App" width="350">
</p>

### Git Clone and Run Docker Container
* Clone the github repository from command line or terminal:
  ```sh
    $ git clone https://github.com/akhanna6/CS410-CourseProject-Team-AEJ.git
  ```
* Go inside CS410-CourseProject-Team-AEJ directory.
  ```sh
     $ cd CS410-CourseProject-Team-AEJ
  ```
* Build the Docker Image *(make a note of . (dot) at the end) – Approx. time to run 2 mins*
  ```sh
     $ docker build -t brandanalyser .
  ```
  <p align="center">
    <img src="./img assets/docker3.png" alt="docker build cmd" width="650">
  </p>
  
 * Run the Docker container
   ```sh
      $ docker run -p 8501:8501 brandanalyser
   ```
  <p align="center">
    <img src="./img assets/docker4.png" alt="docker run cmd" width="650">
  </p>
  
 * To use the software, open the URL which you see once you type *docker run -p 8501:8501 brandanalyser* in your command line. Alternatively, you can also open it by clicking on URL visible inside PORT(S) in Docker Image.
  <p align="center">
    <img src="./img assets/docker5.jpg" alt="brandalalyser} docker image" width="650">
  </p>


### Software Code Structure
* **app.py**: This file has the Dashboard code of our software and is the main file to run the code.
* **helper.py**: All functions are defined inside this file. These are then referenced inside app.py.

### Twitter API Keys (Not Required for Software Testing)
* For Future use, it is recommended to get your own twitter developer API Keys using this [link](https://developer.twitter.com/en/docs/twitter-api/getting-started/getting-access-to-the-twitter-api)
