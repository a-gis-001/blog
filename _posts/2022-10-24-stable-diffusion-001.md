---
title: "Stable Diffusion part 001"
date: 2022-10-24
---

### Patty Donaghy

![c18e77be3a7d48bb920a58c231f739ee](https://user-images.githubusercontent.com/116606542/197654212-4c510dd7-e150-4215-836a-2e87341b84a1.png)

#### Parameters

- Prompt: cousin of John Francis "Jack" Donaghy, tv executive, ornnate, photorealistic, oil painting in the style of clue board game, martini in one hand, other hand in pocket of suit jacket, looking cool but excited
- Model: stable-diffusion
- Model Version: v1.4
- Guidance Scale: 17.9
- Dimensions: 512 x 768
- Seed: 6995560496996294
- Steps: 123
- Sampler: LMS

#### Thoughts on Creation

I really like the oil painting style for rendering something interesting that feels like a completely new and interesting character. However, some of the time you get a picture frame in the image, which makes sense because you asked for an oil painting and I'm sure there's lots of those in the training database and the frame is a part of it. Experiments with using a negative prompt did not seem so successful.

| no negative prompt | negative prompt "frame" |
| ------------------ | ----------------------- |
| ![tmppp7glp5w](https://user-images.githubusercontent.com/116606542/197739303-444b5751-e386-481e-b962-54ec7d9aa560.png)   | ![tmpb6kcru99-noframe](https://user-images.githubusercontent.com/116606542/197739338-4106ac9e-6c06-465b-ac79-dc60cddf533b.png)     |


#### Tools

So the website [ mage.space](https://www.mage.space) is an absolute beast. It is so fun to test different combinations, it runs near instantly. The album they create is also beautiful. Overall, it is really well done. Locally I have a NVIDIA 3060 running https://github.com/AUTOMATIC1111/stable-diffusion-webui.git to explore more.
