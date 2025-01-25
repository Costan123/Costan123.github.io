

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
  <video width="590" height="470" controls>
  <source src="Installing Jupyter Notebook on Ubuntu! 720.mp4" type="video/mp4">
  Your browser does not support the video tag.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Website Analytics</title>
</head>
<body>
  <h1>My Awesome Website</h1>
  <p id="analytics">Loading analytics...</p>

  <script>
    // Replace with your Google Analytics View ID and API Key
    const viewId = "474727906"; // Example: ga:123456789
    const apiKey = "G-9KJYM44VMH";

    // Fetch data from the Google Analytics API
    fetch(`https://analyticsreporting.googleapis.com/v4/reports:batchGet?key=${apiKey}`, {
      method: "POST",
      headers: { "Content-Type": "application/json" },
      body: JSON.stringify({
        reportRequests: [
          {
            viewId: viewId,
            dateRanges: [{ startDate: "7daysAgo", endDate: "today" }],
            metrics: [{ expression: "ga:pageviews" }],
          },
        ],
      }),
    })
      .then((response) => response.json())
      .then((data) => {
        const pageViews = data.reports[0].data.totals[0].values[0];
        document.getElementById("analytics").textContent = `This page has been viewed ${pageViews} times in the past week.`;
      })
      .catch((err) => {
        console.error("Error fetching analytics data:", err);
        document.getElementById("analytics").textContent = "Unable to load analytics.";
      });
  </script>
</body>
</html>


