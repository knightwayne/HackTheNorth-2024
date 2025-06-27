# 🌸 Fleurish

![Main Image](./images/original.png)

**Imagine turning any image into a dynamic animation in just seconds—no design or animation skills needed. With Fleurish, static visuals come to life with a flourish at the press of a button.**

---

## Inspiration

There are a lot of text-to-image, image-to-text AI generators, only a few image-to-video AI generators, but from our research, we couldn't find an AI generator that converted live images to video (.gif). We wanted to fill this void, since it has a few useful applications, and so we created Fleurish!

---

## What it does

When the user inputs an image, selects a theme and clicks the "Imagine" button, an AI-generated gif based on the inputted image will be generated after a few seconds. Alternatively, if the user connects their phone to their computer, they can also use the "live image" option to get the application to read images from the phone camera video in real time.

![Working Demo](./images/original_.png)

---

## How we built it

We used a Convex template with a built-in Replicate integration as our backend, and then added on a Replicate https://replicate.com/lucataco/dreamshaper7-img2img-lcm in order to convert images to AI-generated images. For the live image option, we used RTC peer connections to send camera feed to a Python backend, which then compresses the image (to optimize the AI generation) and feeds to the front-end, built in Next.js with the WebSocket API.

---

## Challenges we ran into

We spent a lot of time testing and searching for a model that gave us satisfactory results, and even then, it took us time to learn how to integrate that with our application. Also, we did not have previous experience with a lot of the technologies used, namely generative AI (with images), WebSocket API, and using the RTC peer connection to allow the communication between a phone and our application.

---

## Accomplishments that we're proud of

Our application is highly optimized and generates the gif within 1–2 seconds. Also, the themes and the gifs produced give very accurate results.

---

## What we learned

We learned a lot of new technologies, such as Convex, WebSocket API and RTC peer connection. We also gained experience with image generative AI, which is vastly different than text generative AI. Also, learning to integrate all of the technologies used together was a very insightful learning experience.

---

## What's next for Fleurish

Better, faster models, user management (so there is no overlap between users).

---

## Built With

- Cohere  
- Convex  
- Next.js  
- Python  
- Replicate  
- WebSocket  

---

## Try it out

- 🔗 **GitHub Repo**: [https://github.com/htn-2024-amtz/HTN-2024](https://github.com/htn-2024-amtz/HTN-2024)  
- 🔗 **Devpost**: [https://devpost.com/software/fleurish](https://devpost.com/software/fleurish)  
- ▶️ **YouTube Demo**: [https://youtu.be/N-FeuSmbEqA](https://youtu.be/N-FeuSmbEqA)
