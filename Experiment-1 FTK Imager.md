# Experiment-1: Evidence Acquisition Using FTK Imager

*Course / Lab:* Digital Forensics Lab  
*Experiment No.:* 1  
*Title:* Evidence Acquisition Using FTK Imager  

---

## Aim
To capture RAM data and create a forensic disk image using FTK Imager.

---

## Requirements
- FTK Imager  
- Windows operating system  

---

## Description
- FTK Imager is a forensic acquisition tool used to create exact copies (disk images) of storage devices.  
- It allows capturing RAM data, entire drives, or specific partitions without altering original evidence.  
- Investigators use it to preview, preserve, and export data for further forensic analysis.  

---

## Part A — Acquiring Volatile Memory (RAM) Using FTK Imager

*Step-1:* Right click on the FTK Imager tool and select *Run as administrator*.  

![images/exp1-disk-step1.png](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/WhatsApp%20Image%202025-09-01%20at%2021.58.15_46523922.jpg)

*Step-2:* On the top menu bar, click *File* and select *Capture Memory* from the drop-down list.  

![(images/exp1-ram-step2.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20203030.png)

*Step-3:* A dialog box will appear. Select the destination path to your file and provide the file name with .mem extension. (Pagefile and AD1 file options are optional.)  

![(images/exp1-ram-step3.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20203149.png)

*Step-4:* Click the *Capture Memory* button to start acquisition of memory.  

![(images/exp1-ram-step4.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20203959.png)

*Step-5:* A progress bar in green colour will indicate the capture status. The time taken to capture RAM depends on the system’s RAM size. After completion, the captured memory file will be available in the chosen destination folder.  

![(images/exp1-ram-step5.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204132.png)
---

## Part B — Acquiring Non-Volatile Memory (Disk Image) Using FTK Imager

*Step-1:* On the top right menu bar, click *File* and select *Create Disk Image* from the drop-down menu.  

![Step 1](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204304.png)
*Step-2:* In the dialog box, choose the source evidence type like *Physical Drive, Logical Drive, Image File, or Contents of a folder*.  

![(images/exp1-disk-step2.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204335.png)

*Step-3:* Select the drive you want to image and click *Finish*.  

![(images/exp1-disk-step3.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204351.png)
*Step-4:* In the *Create Image* dialog, click *Add* to define image type. 

![(images/exp1-disk-step4.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204401.png)

*Step-5:* Select the image type from the dialog box (Raw / SMART / E01 / AFF). Among all, *E01 is recommended*. 

![(images/exp1-disk-step5.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204412.png)

*Step-6:* Fill in the case information (Case Number, Evidence Number, Examiner Name, Unique Description, Notes) and click *Next*.  

![(images/exp1-disk-step6.png)](https://github.com/SaicharanT-tech/Digital-Forensics-Lab-Exercises-/blob/c28d613b91ddb4dcb3005f5081b4f8077e34cd1c/Images/Screenshot%202025-09-01%20204609.png)

*Step-7:* Choose the destination folder and give a file name for the image.  

![(images/exp1-disk-step7.png)](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/88dd3dcf55bf6caaf1833c97ad1758f771348668/images/WhatsApp%20Image%202025-09-01%20at%2012.17.38.jpeg)

*Step-8:* Set options like compression, splitting size, and click *Finish. After that, click **Start* to begin the imaging process.  

![(images/exp1-disk-step8.png)](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/88dd3dcf55bf6caaf1833c97ad1758f771348668/images/WhatsApp%20Image%202025-09-01%20at%2012.18.06.jpeg)


FTK Imager will display progress along with hash values. The imaging process may take time depending on the drive size. After completion, FTK Imager verifies the hash values automatically to maintain forensic integrity. Finally, the hash values should match.  

---
