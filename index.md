**Smart Mirror**

This project transforms a traditional bathroom mirror into a multifunctional smart display. By integrating a digital screen, the system mimics the appearance of a standard mirror while offering smartphone-like features such as displaying the time, weather updates, calendar events, and personalized medication reminders. These modifications transform the standard bathroom mirror into a personal assistant.  It is especially beneficial for individuals who take regular medication, providing consistent and timely reminders each time they enter the bathroom improving their overall wellness!

| Name: |School| Area of Interest | Grade |
|:--:|:--:|:--:|:--:|
| Triya S | Foothill High School | Computer Science | Incoming Junior

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# **Final Milestone**

<iframe ADD </iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
For my final milestone, I have successfully created my medicine reminders module, as well as added a module for . My biggest triumphs included getting my . Through this process, I have learnt: how to use a raspberry pi display and how to install a camera feature into it, how to operate in the command prompt and use linux commands, how to format a website and how to embed and create my own modules. In the future, I hope I can further expand on my knowledge of python and use of the command prompt terminal! 


- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# **Second Milestone**

<iframe width="560" height="315" src="https://www.youtube.com/embed/_eKFbrD7Oyw?si=GT7kiSxQ37nz4TtB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Since completing my base project, I have focused on creating a live camera feed to show on my display screen. Surprisingly, this has been the most time consuming and confusing task yet. Inserting the white ribbon camera took me 20 minutes since I had trouble pushing the grey clip down with the ribbon inserted. Eventually, pushing down one side at a time solved this error. I also experienced problems with the software. I tried five different code segments regarding embedding a live stream straight on to my display screen. None of these segments worked, but eventually with some support I was able to add code which could display the live feed on a website. I have adapted and displayed this website as full screen on my display to act as a mirror. Before my final milestone, I need to create my own module to add reminders, add my google doc module and find a way to display all of the above with the basic MagicMirror module. 

# **First Milestone**

<iframe width="560" height="315" src="https://www.youtube.com/embed/M68OSya9c-o?si=nQ-mRqXoc6oYmflQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


My plan for the Smart Mirror is to use a raspberry pie operating system with a camera attached to connect a display screen. For my first milestone, I have finished the base for my project which includes: connecting HDMI and USB cables to the display from the raspberry pi, connecting the wireless mouse and keyboard to the raspberry pi and using command prompt on my computer to ssh into my raspberry pi to open the MagicMirror module on my display screen. I've faced many challenges, mostly with the hardware since the raspberry pi is very delicate and it was hard for me to attach all the cables. I've learnt to hold the back of the cable slot on the bread board firmly and slightly twist the cable while pushing it in. I also faced troubles with  software, since it took a while to install the MagicMirror application. I continuosly recieved errors where my computer could not establish the authenticity of my raspberry pi. I learned to  use sudo infront of the install command to troubleshoot this error. This error occured as the computer inherently protects itself from unknown application and the sudo statement can overrride this. My plan for the future is to install the camera in so I’ll be able to see myself through the display and it will operate as a mirror and Additionally, I would like to add in a module for google doc notes and possibly sports, as well as create my own module for reminders!

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code

```{
			module: 'MMM-MedicineReminder',
			position: 'top_center',
			config: {
				foo: "Reminder: Take your medicine",
				phrases: ["Did you have enough water today?", "Hey buddy, you should have some water!","Drink water, bro.","'Better to have stones in the way than in the Kidneys: Drink water!'",
				"It's been such a long time since your last glass of water...","Water! Water! Water!","Are you anxious for the next glass of water?"],
				additionalPhrases: [],
				startTime: "00:00",
				endTime: "23:59",
				messageDuration: 1 * 60 * 1000, // 1 min showing on the screen
				animationSpeed: 4 * 1000, // 4 seconds for fading
				reminderFrequency: 1 * 60 * 1000, // hourly reminder
				classes: "bright medium light",
				color: "#fff",
				idleMessage: "<br/>",
				logo: true,
				days: [0,1,2,3,4,5,6], // all week
				alarm: {
					status: false, 
					daysWithAudibleReminder: [1,2,3,4,5],
					src: "done-for-you.mp3",
					startTime: "09:00",
					endTime: "17:00",
				}
			}
		},
```

# **Bill of Materials**

Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| RasTech Raspberry Pi Starter Kit | Used for connecting the display to the camera and operating the display. | $103.99 | <a href="https://www.amazon.com/RasTech-Raspberry-Starter-Heatsink-Screwdriver/dp/B0C8LV6VNZ/ref=sr_1_4?crid=3506HY00MCGVM&dib=eyJ2IjoiMSJ9._zkM62vSQ8p7tNr88715LdMv_qHh72Je-tkF9PXEa3chDE53QT4aZu4AGAb4ihE61QY4ZD55nKF6Fp2Kfs8t7AbafM_JrlJFfHo9OB4eAVGqa0EB-7aoBQHPmhKHZ2MW8ny-Kd44bMVlVxPlTWVk5YHIN5P3uKVqrE5Dcal0rKkHny-O6Xyb5ux2AOU6OwVbkag_bqBX66RQNRrgBuz-0pS43mcx93IZTQA9R8NaJJypYU2HAycp-XicTFmyU60a01Nfm9iuyo6B9yA8ppN3OQQyJ-NQ9xyNPxfTLwkqtng.yAYpU6outhQcZmOZhN9Wb6yTw7A85CNUbXZguGInZNg&dib_tag=se&keywords=raspberry%2Bpi%2Bkit&qid=1718848547&s=electronics&sprefix=rasbperry%2Bpi%2Bkit%2Celectronics%2C83&sr=1-4&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Wireless Keyboard | Operates the display. | $21.99 | <a href="https://www.amazon.com/gp/product/B07XDWCLYF/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| 7 Inch IPS LCD Touch Screen Display Panel  | Displays the smart mirror and camera feature. | $39.99| <a href="https://www.amazon.com/Hosyond-Display-1024%C3%97600-Capacitive-Raspberry/dp/B09XKC53NH/ref=sr_1_3?crid=1KKB9WC62OIAD&keywords=raspberry%2Bpi%2Bips&qid=1685911698&s=electronics&sprefix=raspberry%2Bpi%2Bips%2B%2Celectronics%2C87&sr=1-3&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
| Adapter and Sd card Reder | Used for operating the raspberry pi. | $9.99 | <a href="https://www.amazon.com/dp/B081VHSB2V?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1"> Link </a> |
|:--:|:--:|:--:|:--:|
# **Other Resources/Examples**
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- https://www.howtoraspberry.com/2022/02/real-time-streaming-protocol-and-the-raspberry-pi-video-for-linux-2/
- https://docs.magicmirror.builders/development/introduction.html#general-advice
