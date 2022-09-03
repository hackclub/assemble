# 👏 Judging

When planning Assemble, we knew a system for judging and prizes was needed. Judging gives attendees feedback and recognition for their project, and prizes, even if small, provide something to work toward and receive for hard work. With that in mind, we got into the mindset of brainstorming more innovative and fun judging options than what you’d typically find at a hackathon, leaving that as a fallback in case we couldn’t come up with something. 

Some ideas for judging included, ranked choice, upvoting, and emoji reactions. One of those would be paired with our ideas for demoing projects: either group presentations, speed dating, scrapbook gallery, or science fair style. We ended up deciding on a science fair style demonstration and emoji reaction judging system. The science fair demonstrations allowed attendees to meet face to face, try out projects, and interact, rather than just talking to 1 person at a time or waiting for long demos. The emoji reactions system was also appealing to us, as it provided a way for people to judge projects with personality, rather than categorizing them as good, bad, or somewhere in between.

After deciding on judging and presentation systems, we needed a way to pull them together. This is how ship cards were born! The original concept of ship cards included a title, description, image, and collaborators on physical 4x6 photo-paper cards. Each of these would be stationed at 
their respective project demos, and could be scanned with a QR code or NFC tag allowing attendees to select 5 emojis that best fit a project. They would get printed automatically after every ship. This would all tie into Assemble Scrapbook, one place where all attendees could scrapbook mini updates throughout the event and post a ship once they finish. After the lightning project demos, everyone would be released to start exploring and sharing their projects.

<img width="500" alt="Screenshot 2022-09-03 at 7 29 23 PM" src="https://user-images.githubusercontent.com/39828164/188268379-bed3a733-3657-4998-8fd5-33badd2db875.png">

At least, that was the plan. Certain compromises had to be made, such as using cardstock instead of photo paper and printing out the cards at the end instead of automatically. Additionally, some things didn’t go quite right at the event, if they were even finished. Certain components like the printer driver, screenshooting API, and project numbering system weren’t tailored to fit Assemble’s use case and weren’t ready to scale.During the last 3 hours of the event, Assemble Scrapbook received over 15 million database requests. This brought the system entirely offline, as it was built on Vercel Serverless Functions and the Postgres database requests weren’t connection pooled. It took us about 30 minutes to fix just the database request pooling alone. 

<img width="500" alt="Screenshot 2022-09-03 at 7 31 27 PM" src="https://user-images.githubusercontent.com/39828164/188268437-c30e24d0-8727-41d8-a0ba-b843c7c06d59.png">

_(praying for the fix to work, spoilers: it caused a new bug)_

Once we had Scrapbook back up, it was time to initiate printing! This was a nightmare, given that we had about 45 minutes to send all ship card images to my laptop for printing, cut each card out, and affix an NFC tag to the back. It wouldn’t have been possible without help from Max, Gary, Celeste, and Kognise. The last ship card rolled off of the printer right as lightning demos wrapped up. With everything finally set up and configured, attendees grabbed a ship card for their project and started exploring.

<img width="500" alt="Screenshot 2022-09-03 at 7 28 24 PM" src="https://user-images.githubusercontent.com/39828164/188268344-4d19f7b7-02d4-4063-893c-85c619767b5f.png">

As the emoji reactions rolled in, we paired projects with ideal awards. For example, the project with the most upvotes receive the Most Upvoted award! And other projects like The Big Brain award and Most Polished Project were determined by the number of emojis related to the respective topics, like a brain or sparkles. Then we presented each group with their awards, and concluded Assemble with a short talk from Sam and Zach and a group photo.

<img width="500" alt="Screenshot 2022-09-03 at 7 29 56 PM" src="https://user-images.githubusercontent.com/39828164/188268394-847b9299-3d0a-4f93-92ad-b49b7c738acd.png">

