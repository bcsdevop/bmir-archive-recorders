# BMIR Internet Radio Archive Recorders

This project contains the scripts to install and configure several different internet radio archive recorders used at Burning Man Information Radio (BMIR 94.5 FM), at the annual Burning Man festival, in Black Rock City, Nevada, USA.

Several tools and techniques have been used to record the archives over the years.  As they have grown more diverse and complicated, his github project was created to store and share the scripts.


![Image of BMIR](https://raw.githubusercontent.com/sagittandy/bmir-archive-recorders/master/pix/bmir.archivers.2017.png)


## Studio Icecast + Streamripper

These two processes will run on one standalone Ubuntu Linux computer in the studio.  Orban Opticodec will 'upload' a digitized music stream to this icecast2 server (in addition to uploading to several music servers on the public internet.).  Streamripper 'listens' to the stream from icecast and records it to mp3 files.

This technique is new and experimental at Burning Man 2017.

## Studio TotalRecorder

A Behringer UMC204HD Audio Interface in the studio digitizes baseband audio from the studio mixer and transfers it via USB cable to an HP desktop computer in the studio.  The computer runs Windows 7 and commercial audio recorder software TotalRecorder.  http://www.totalrecorder.com/  TotalRecorder is configured to repeatedly record audio to mp3 files in 2-hour segments, synchronized with clock time.  MP3 files are manually copied to USB thumb drive daily, to provide backups.  Note:  This computer does not have antivirus software installed and is intentionally never connected to the internet.  TotalRecorder was first used in 2016.

## Android FM Recorder

A Motorola Moto-E android smartphone is used to record BMIR off-air.  The Moto-E contains internal FM receiver hardware.  An FM radio app authored by Motorola was installed.  The app free-runs continuously, and is set up to store AAC files to micro-SD memory chip.  The recorder app is manually stopped and immediately restarted every 6-12 hours to split the AAC files into manageable size.  The phone was powered by a 12-volt battery (UB12120) and 5v USB charger, housed in a Harbor Freight ammo box (#61451), in the archivist's tent.  It was first used in 2016.

## Offsite Streamripper

Streamripper has been run on an Ubuntu Linux VM at Digital Ocean for many years (starting 2010?).  It is configured to record mp3 files in 4-hour segments (unsynchronized to clock time).  It works well, but is subject to frequent outages due to the unreliable connection between the studio at Burning Man and internet routers in the default world.
