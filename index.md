---
title: Costin Neagoe
description:  Sports Photographer / Cinematic Videographer, Computer Engineering Student
---

<p align="center">
    <a href="https://mail.google.com/mail/u/0/?fs=1&to=788513@pdsb.net&tf=cm">Contact Me - costin.neagoe@yahoo.com</a>
</p>

#  My Pictures and Videos
- ### Sports Photography
  - Over my time at Port Credit, i've developed a love for photography. Click the Link to see different picturse that i've taken of players from Football, Rugby, Kayaking/Canoeing and Long Distance runners.
  [Link](https://drive.google.com/drive/folders/15K9dY2IpA7PAkg2Fk9Cazenigmi4cxP5?usp=drive_link)
![e](IMGL6347.jpg)

- ### Cinematic Videos
  - Adding onto my liking of photography, I purchased a drone and started using it to film cinematic videos. Follow the link or click the video to check them out.
  [Link](https://drive.google.com/drive/folders/1-2kOdHDsvPd6vPiCYo6j8hLZmPwcIxvy)
<video width="590" height="390" controls>
  <source src="copy_6ADF3497-8841-4272-A835-B51B0F4CD40F(2)(1)(2)(2).mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

  
# Stock Programs
- ### Single Stock Viewer 
  - View one singular stock through Jupyter Notebook. Must have Linux and Jupyter Notebook installed for link to work.
    [Link](http://localhost:8888/notebooks/SINGLE.ipynb)

- ### Multiple Stock-Viewer 
  - View multiple stocks through Jupyter Notebook. Must have Linux and Jupyter Notebook installed for link to work.
    [Link](http://localhost:8888/notebooks/workingstockwithmultiple.ipynb)

- ### Stock Ticker Names
    - Follow the link to view the ticker of any major company's stock.
      [Link](https://stockanalysis.com/stocks/)

- ### How to install Jupyter Notebook on Linux
   -Click on the video to see a step-by-step tutorial on how to download Jupyter Notebook on Linux-Ubuntu.
  <video width="590" height="490" controls>
  <source src="Installing Jupyter Notebook on Ubuntu! 720.mp4" type="video/mp4">
  Your browser does not support the video tag.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Visitor Counter</title>
</head>
<body>
  <h2>Visitor Counter</h2>
  <p id="visitor-count">Loading...</p>

  <script>
    // API URL for countapi.xyz
    const apiUrl = "https://api.countapi.xyz/hit/costan123.github.io/visits";

    // Fetch the count and display it
    fetch(apiUrl)
      .then(response => response.json())
      .then(data => {
        document.getElementById("visitor-count").textContent = 
          `This page has been visited ${data.value} times!`;
      })
      .catch(err => {
        console.error("Error fetching visitor count:", err);
        document.getElementById("visitor-count").textContent = "Unable to load visitor count.";
      });
  </script>
</body>
</html>
