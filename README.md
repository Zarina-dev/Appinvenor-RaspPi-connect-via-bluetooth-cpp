# Connect Appinventor app with RaspPi via bluetooth (Raspberry pi 4, c++)

# Data flow:
(check to see  <a href="https://www.youtube.com/shorts/GnplWsxTpzo">video result in youtube</a>)

<img width="598" alt="image" src="https://user-images.githubusercontent.com/61898376/220945981-c4fcda60-e08f-4ce9-afee-d9a10a0ef008.png">


# 1. Code Preparations

## a. Android mobile & Raspberry pi Pairing
before starting a mobile Device which will install app inventor App and raspberry pi **should be paired**

I referenced this page: <a href="https://webnautes.tistory.com/1137">in Korean</a>

## b. raspberri pi  (server)

**Used:**

raspberry pi: raspberry pi 4 model b

IDE: Visual Studio Code

language: c++

packages: wiringPi (should be installed before running c++ code)

---

**Build c++ file:**

1. Open terminal, go to folder 
2. input this commands:
```
pi@raspberrypi:~FOLDER_PATH $ g++ -o main1 main.cpp -lbluetooth -lpthread
pi@raspberrypi:~FOLDER_PATH $ ./main1     // will be listening to client 
```


## c. app inventor App (Mobile)

**import .aia file:**

 1. in PC <a href="https://appinventor.mit.edu/"> Go to App inventor site </a>
 2. click 'Create Apps'   
 3. click 'Project' tab
 4. click 'Import project (.aia) from my computer'
 5. upload ```appInventorApp.aia``` file
 

---
 
**install app inventor App to mobile:**

  1. [in MOBILE] download **MIT AI2 Companion** app from google store
  2. [in PC - MIT APP INVENTOR page]  ```Connect``` >> ```AI Companion``` >>> QR code window will be open
  3. [in MOBILE - MIT AI2 Companion] ```scan QR code``` >>> scan QR
  
  
  
---

# 2. Result

## a. app inventor App

![image](https://user-images.githubusercontent.com/61898376/220891411-34142ede-7d0f-453e-9b96-8c82fee4af4b.png)

## b. raspberri terminal

<img width="596" alt="image" src="https://user-images.githubusercontent.com/61898376/220912560-406da4fe-666e-486b-843b-01a4407071a2.png">

## c. result video
<a href="https://www.youtube.com/shorts/GnplWsxTpzo">Youtube</a>
